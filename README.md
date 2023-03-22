# ansible-role-actions-runner
Ansible Role - GitHub Actions Runner

## Role Variables
Available variables are listed below, along with default values (see `defaults/main.yml`):

```yml
github_pat: "token"
github_organization: "organization"
```

## Add to `requirements.yml`

```yml
roles:
  - name: soramitsukhmer-lab.actions-runner
    src: https://github.com/soramitsukhmer-lab/ansible-role-actions-runner
    version: main
    scm: git
```

## Use with Ansible

Example:

```yml
- hosts: all
  become: true
  vars:
    github_pat: "your-github-token-here"
    github_organization: "your-github-organization"
  roles:
    - soramitsukhmer-lab.actions-runner
```
