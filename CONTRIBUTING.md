# Contributing to veeam-ansible

## Ansible Standards

### Required Playbook Header

Every playbook must begin with a comment header including Playbook name, Description, Author, Date, Version, and Repo.

### Credential Rules

- Use `ansible-vault` for all sensitive values
- Variable naming convention: `vault_<vendor>_<field>`
- Always set `no_log: true` on tasks that use credentials

### Lint Compliance

All playbooks must pass `ansible-lint` before merging:

```bash
ansible-lint <playbook.yml>
```

## Commit Prefixes

`add`, `fix`, `docs`, `update`, `remove`, `refactor`
