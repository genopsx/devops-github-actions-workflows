# DevOps Shared Workflows

This repo contains a collection of shared, versioned workflows for use on Terraform modules.

It's maintained by the DevOps team, but we welcome PRs from anyone!

To use the files in this repo, aim your workflow at them using the following methodology:

```
name: Terraform module tests

on:
  workflow_call:

jobs:
   terraform-test:
     runs-on: self-hosted
     uses:
       genopsx/devops-github-actions-workflows/terraform/terraform_module_test.
       yml@main
```

We encourage you to be explicit about the branch or release.  Versioning of this repo is coming soon (TM).


To-do:

- Add semantic versioning to this repository for releases via GitHub Actions.
- Add semantic versioning as a reusable workflow to be pulled into other workflows.
