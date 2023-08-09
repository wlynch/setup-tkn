# GitHub Action for Tekton

This GitHub Action configures [`tkn`](https://github.com/tektoncd/cli) in the
environment for managing [Tekton](https://tekton.dev/) resources in GitHub
Actions.

Tekton is a powerful yet flexible Kubernetes-native open-source framework for
creating continuous integration and delivery (CI/CD) systems. It lets users
build, test, and deploy across multiple cloud providers or on-premises systems
by abstracting away the underlying implementation details.

This repo was originally forked from https://github.com/jerop/tkn

## Usage

`wlynch/setup-tkn` installs `tkn` for your operating system

```yaml
- uses: wlynch/setup-tkn@main
```

## Version

`wlynch/setup-tkn` installs the latest version of `tkn` by default - use
`version` to select a specific version of `tkn`

```yaml
- uses: wlynch/setup-tkn@main
  with:
    version: v0.18.0
```

## Connecting to clusters

- [GCP](https://github.com/google-github-actions/auth)
- [AWS](https://github.com/aws-actions/configure-aws-credentials)