# `.github`

This is the organization-level **`.github`** repository. The files here provide
**default community-health files and shared configuration** that apply to every
repository in the organization that does not define its own.

> ⚠️ This repository is **public**. Do not commit secrets, credentials, or
> personal data. See [CONTRIBUTING.md](CONTRIBUTING.md).

## What's here

| Path                          | Purpose                                                        | Inherited org-wide? |
| ----------------------------- | -------------------------------------------------------------- | ------------------- |
| `profile/README.md`           | Public landing page shown on the organization's GitHub profile | n/a (org profile)   |
| `ISSUE_TEMPLATE/`             | Default bug-report and feature-request forms                   | ✅ Yes               |
| `PULL_REQUEST_TEMPLATE.md`    | Default pull-request template                                  | ✅ Yes               |
| `CONTRIBUTING.md`             | How to contribute                                              | ✅ Yes               |
| `CODE_OF_CONDUCT.md`          | Expected behavior and enforcement                              | ✅ Yes               |
| `SECURITY.md`                 | How to report vulnerabilities                                  | ✅ Yes               |
| `SUPPORT.md`                  | Where to get help                                              | ✅ Yes               |
| `workflows/secret-scan.yml`   | Reusable secret-scanning workflow (callable by other repos)    | Callable, not auto  |

## Notes on inheritance

- **Community-health files** above are used by any org repo that lacks its own copy.
- **Reusable workflows** are *not* applied automatically — a repo must call them
  explicitly (see the header of `workflows/secret-scan.yml`).
- **Dependabot config and `CODEOWNERS` do not inherit** from this repository;
  they must be defined per-repo. They are intentionally omitted here.