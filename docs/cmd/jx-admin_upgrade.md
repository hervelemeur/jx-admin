## jx-admin upgrade

Upgrades your environment git repository to use the latest helm 3 / helmfile and version stream

### Usage

```
jx-admin upgrade
```

### Synopsis

Upgrades your environment git repository to use the latest helm 3 / helmfile and version stream

### Examples

  # upgrades your current environment's git repository
  jx-admin upgrade

### Options

```
      --approver stringArray                the git user names of the approvers for the environments
  -b, --batch-mode                          Enables batch mode which avoids prompting for user input
  -d, --dir string                          The directory used to create/clone the development git repository. If no directory is specified a temporary directory will be used
      --env-git-owner string                the git owner (organisation or user) used to own the git repositories for the environments
      --git-credentials                     initialise the git credentials so that this step can be used inside a Job for use with private repositories
      --git-kind string                     the kind of git repository to use. Possible values: bitbucketcloud, bitbucketserver, gitea, github, gitlab
      --git-name string                     the name of the git repository
      --git-server string                   the git server host such as https://github.com or https://gitlab.com
      --git-token string                    the git token used to operate on the git repository
  -g, --git-url string                      The git repository to clone to upgrade
  -h, --help                                help for upgrade
      --initial-git-url string              The git URL to clone to fetch the initial set of files for a helm 3 / helmfile based git configuration if this command is not run inside a git clone or against a GitOps based cluster (default "https://github.com/jenkins-x/jx3-boot-config.git")
      --latest-release                      upgrade to latest release tag
      --out string                          the name of the file to save with the created git URL inside
      --repo string                         the name of the development git repository to create
      --upgrade-version-stream-ref string   a version stream ref to use to upgrade to (default "master")
      --use-pr                              If enabled lets force the use of a Pull Request rather than creating a new git repository for the helm 3 based configuration
```

### SEE ALSO

* [jx-admin](jx-admin.md)	 - commands for creating and upgrading Jenkins X environments using GitOps

###### Auto generated by spf13/cobra on 1-Oct-2020
