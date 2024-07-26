<!--
SPDX-FileCopyrightText: Contributors to the IEEH TU Dresden software project

SPDX-License-Identifier: MPL-2.0
-->

# How to Contribute

We'd love to accept contributions to these projects in any forms. 
You do not need to be a programming or power system expert to make a contribution.
There are just a few small guidelines you need to follow before making a change.


## General Recommendations for Contributing

Contribution does not necessarily mean committing code to the repository. 
We recognize different levels of contributions as shown below in increasing order of dedication:

1. Test and use the libraries. Give feedback on the user experience or suggest new features.
2. Validate the model against other existing libraries. Provide validation test cases.
3. Report bugs.
4. Improve the Python interface or helper functions.
5. Contributing to the Python core
    1. Develop new mathematical algorithms
    1. Improve or add new features into the Python codebase

A good place to start is to look at issues with the `good first issue` label, or to check the [PowerFactory Tools](https://github.com/ieeh-tu-dresden/powerfactory-tools) project.


## Filing bugs and change requests

You can file bugs against and change request for the project via GitHub issues. 
Consult [GitHub Help](https://docs.github.com/en/free-pro-team@latest/github/managing-your-work-on-github/creating-an-issue) for more information on using GitHub issues.
Please consider [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)) in general.


## Community Guidelines

This project follows the following [Code of Conduct](CODE_OF_CONDUCT.md).


## Style Guide

For Python code we use the pipeline to automatically check the formatting.
We use `black` and `ruff` to check Python code.
If the code format is not complying, the pipeline will fail and the pull request will be blocked.

### Python

This project uses the PEP 8 Style Guide for Python Code. For all details about the various conventions please refer to [PEP 8](https://www.python.org/dev/peps/pep-0008).

Tip: Use [black](https://github.com/psf/black) to automatically format your Python code to conform to the PEP 8 style guide.

Furthermore, the following conventions apply:

* Maximum line length: 120 characters
* Double quotes for strings, keys etc.
    * Except when double quotes in the middle of a string are required.


## Git branching

Our projects use the [GitHub flow Workflow](https://guides.github.com/introduction/flow/) and branching model. 
The `main` branch always contains the latest tested code. 
New feature/fix branches are branched from `main`. 
When a feature/fix is finished, it is merged back into `main` via a [Pull Request](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

In case all referred issues within a milestone are completed, a patch version (release) is generated.

## Issue and Pull Request Process
Contributions should be submitted as Github pull requests. 
See [Creating a pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) if you're unfamiliar with this concept.
Please make sure that the issue or pull request starts with a valid prefix (as specified by [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)) and the issue title is in English and lowercase (including the first word after the colon).

The process for a code change and pull request you should follow:

**Using a fork of a project:**
1. Create a topic branch in your local repository, following the naming format
"feature/###" or "fix/###". 
For more information see the Git branching guideline.
2. Make changes, compile, and test thoroughly. 
Ensure any install or build dependencies are removed before the end of the layer when doing a build. 
Code style should match existing style and conventions, and changes should be focused on the topic the pull request will be addressed. 
For more information see the style guide.
3. Push commits to your fork. 
Please use [default commit message style](https://www.conventionalcommits.org/en/v1.0.0/)

**Using a issue template from the projects github page:**
1. Create an issue, choose one of the templates and follow the instructions given there.
2. Make changes, compile, and test thoroughly. 
Ensure any install or build dependencies are removed before the end of the layer when doing a build. 
Code style should match existing style and conventions, and changes should be focused on the topic the pull request will be addressed. 
For more information see the style guide.
3. Push commits to your issue branch.
Please use [default commit message style](https://www.conventionalcommits.org/en/v1.0.0/)

4. Create a Github pull request from your topic branch.
5. Pull requests will be reviewed by one of the maintainers who may discuss, offer constructive feedback, request changes, or approve the work. 
For more information see the remark to code review below.
6. Upon receiving the sign-off of one of the maintainers you may merge your changes, or if you
   do not have permission to do that, you may request a maintainer to merge it for you.

### pre-commit hooks

Thise projects use `pre-merge-workflows` to run a list of checks (and perform some automatic corrections) to your code (style) before each commit.
It is up to the developer to choose whether you would like to use this tool or not.
The goal is to make sure, that each commit will pass the quality checks in the github actions workflow.

You can manually run checks whenever you like:
```bash
black .
ruff check .
mypy .
```

### Code reviews

All patches and contributions, including patches and contributions by project members, require review by one of the maintainers of the project. 
We use GitHub pull requests for this purpose. 
Consult the pull request process below and the [GitHub Help](https://help.github.com/articles/about-pull-requests/) for more information on using pull requests.

## Attribution

This Contributing.md is adapted from Google available at https://github.com/google/new-project/blob/master/docs/contributing.md