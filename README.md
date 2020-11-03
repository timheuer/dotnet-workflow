![Build](https://github.com/timheuer/dotnet-workflow/workflows/Build/badge.svg)

# `dotnet new workflow`
This is a simple global tool to give you a handy and quick method to create a GitHub Actions workflow file for continous integration (CI) builds.

## Usage
To create a workflow for your project from the root of your source code (which would represent the root of your repo -- GitHub Actions workflows exist in the root of your repo).  Some examples

### Default
To use all the defaults:

`dotnet new workflow`

This generates the workflow with all the defaults:
- latest SDK version using Major.Minor.x versioning (e.g., `3.1.x`)
- workflow file will use project name
- default branch of `main`

### Custom options
To specify the name of your YAML file and/or the SDK version you want to use specify more options:

`dotnet new workflow --sdk-version 3.1.403 -n build -b your_branch_name`