# Versioning and Release Guidelines

This document details the versioning, release plan and release guidelines for k0rdent. Stability
is a top goal for this project, and we hope that this document and the processes
it entails will help to achieve that. It covers the release flow, tracking, process, versioning
numbering, support horizon.

This document will be considered a living document. Scheduled releases, supported timelines, and API stability guarantees will be updated here as they
change.

If there is something that you require or this document leaves out, please
reach out by [filing an issue](https://github.com/k0rdent/k0rdent/issues).

-   Docker images with release tags are pushed upon creation of a github release 

-   The release flow consists of the following steps:

    -   Sprint Planning based on backlogs & feature requests from the community
    -   Feature Development with unit-tests & integration/bdd (behaviour driven development) tests
    -   Code/Enhancement freeze with release branch & RC1 (Release Candidate) creation
    -   User & Dev Documentation
    -   Cherry pick of commits from master (fixes) to release branch
    -   Doc sanity tests
    -   k0rdent release with change log

## Releases

Releases of k0rdent will be versioned using dotted triples, similar to
[Semantic Version](http://semver.org/). For the purposes of this document, we
will refer to the respective components of this triple as
`<major>.<minor>.<patch>`. The version number may have additional information,
such as alpha, beta and release candidate qualifications. Such releases will be
considered "pre-releases".

### Major and Minor Releases

Major and minor releases of k0rdent will be made from master. Releases of
k0rdent will be marked with GPG signed tags and announced with the release notes. The tag will be of the
format `<major>.<minor>.<patch>` and should be made with the command `git tag
-s <major>.<minor>.<patch>`.

After a minor release, a branch will be created, with the format
`release-<major>.<minor>.x` from the minor tag. All further patch releases will
be done from that branch. For example, once we release `1.0.0`, a branch
`release-1.0.x` will be created from that tag. All future patch releases will be
done against that branch.

### Pre-releases

Pre-releases, such as alphas, betas and release candidates will be conducted
from their source branch. For major and minor releases, these releases will be
done from main. For patch releases, these pre-releases should be done within
the corresponding release branch.

While pre-releases are done to assist in the stabilization process, no
guarantees are provided.

### Upgrade Path

The upgrade path for k0rdent will be defined soon.

### Next Release

The activity for the next release will be ad-hoc at the start depending on the maintainers discretion followed by a regular release cadence with issues being listed on a project board and being resolved. If you want your issue or PR to be present in the project board (in case unavailable), please reach out to the maintainers or discuss the same on the #k0rdent slack channel  to create the milestone or add an issue or PR to an existing milestone.

