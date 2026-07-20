# Git Lab Repository

This repository contains Terraform and Ansible automation code for infrastructure and deployment workflows.

## Project overview
- Terraform module development for infrastructure building
- Ansible playbook development for Python application provisioning
- Branching strategy and release workflow documentation

## Branch strategy
- `main` branch: production-ready code and hotfix merges
- `dev/july26`, `dev/aug26`: development branches for feature work
- `release/july26`, `release/aug26`: release branches for stabilization
- Feature branches created from the current development branch
- Hotfix branches created from `main`, merged back to `main`, then deleted

## Current work items
- Develop Terraform module [#devops-123]
- Develop Ansible Module [#devops-456]
- Create EKS module in Terraform [#devops-789]
- Create Ansible Python playbook [#devops-987]
- Update Terraform EKS module hotfix [#devops-654]
- Update Ansible playbook hotfix [#devops-313]

## Git ignore sample
The following `.gitignore` content is also included in this repository to keep generated files and local editor files out of source control.

```gitignore
# Terraform files
.terraform/
*.tfstate
*.tfstate.backup
*.tfvars
crash.log

# Ansible files
*.retry
*.vault

# Python files
__pycache__/
*.pyc
*.pyo

# Editor and OS files
.vscode/
*.log
*.swp
Thumbs.db
.DS_Store
```
