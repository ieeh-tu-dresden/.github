<!--
SPDX-FileCopyrightText: Contributors to the IEEH TU Dresden software project

SPDX-License-Identifier: MPL-2.0
-->

# Release strategy

This projects use a *patch release* strategy on the `main` branch.
A milestone context will collect all new pushes (merges) to the `main` branch and - if completed - trigger the release pipline. 
Within the release pipeline GitHub Actions automatically 
build and upload a new version to PyPI with a unique version number.

**All the bug fixes will be committed directly into the `main` branch and published in the latest release. 
No effort will be spent on backporting bug fixes to previous versions!**

## Actively supported Python versions

Core Python libraries in this project are released for Python versions specified in the `pyproject.toml` of the related repository.
