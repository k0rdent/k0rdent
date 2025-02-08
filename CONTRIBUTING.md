# Contributing to k0rdent Projects

Thanks for your interest in contributing to k0rdent and help improve the project! ⚡️✨

This document explains the common procedures expected by contributors while submitting code to k0rdent projects.

We welcome contributions of all kinds

- Development of features, bug fixes, and other improvements.
- Documentation including reference material and examples.
- Bug and feature reports.

  

Fixes and improvements can be directly addressed by sending a Pull Request on GitHub. Pull requests will be reviewed by one or more maintainers and merged when acceptable.
We ask that before contributing, please make the effort to coordinate with the maintainers of the project before submitting large or high impact PRs. This will prevent you from doing extra work that may or may not be merged.
Use your judgement about what constitutes a large change. If you aren't sure, send a message to the **#respond-now** slack or submit an issue on GitHub.



## Code of Conduct

Please read and abide by the [k0rdent Community Code of Conduct](https://github.com/k0rdent/community/blob/main/CODE_OF_CONDUCT.md)

## Submitting Feature Requests

We welcome suggestions to improve the k0rdent project. To ensure a smooth and collaborative process, please follow these steps:

1. **Initiate a Discussion**

   - **Purpose:** Before formalizing a feature request, engage with the community to refine your idea.
   - **Action:** Navigate to the [Discussions](#) tab and start a new topic under the 'Feature Requests' category.
   - **Benefit:** Gather feedback, explore alternatives, and assess interest, increasing the likelihood of acceptance.

2. **Submit a Formal Feature Request**

   - **Prerequisite:** After a fruitful discussion and community support.
   - **Action:** Open a new issue in the [Issues](#) section.
   - **Template:** Select the 'Feature Request' template to provide structured information.
   - **Label:** Apply the `enhancement` label to your issue.

**Note:** Engaging in discussions first fosters collaboration and increases the chances of your feature being integrated.

## General workflow

Identify which part of k0rdent interests you for contributing before starting your contribution journey. Users are requested to raise GitHub issues specific to the repositories you are contributing to.
Once a github issue is accepted and assigned to you, please follow general workflow in order to submit your contribution:
1. Fork the target repository under your github username.
2. Create a branch in your forked repository for the changes you are about to make.
3. Commit your changes in the branch you created in step 2. All commits need to be signed-off. Check the [legal](#legal) section bellow for more details.
4. Push your commits to your remote fork.
5. Create a Pull Request from your remote fork pointing to the HEAD branch (usually `master` branch) of the target repository.
6. Check the github build and ensure that all checks are green.

## Legal

k0rdent Project uses Developer Certificate of Origin ([DCO](https://github.com/apps/dco/)).

Please signoff your contributions by doing ONE of the following:
* Use `git commit -s ...` with each commit to add the signoff or
* Manually add a `Signed-off-by: Your Name <your.email@example.com>` to each commit message.

The email address must match your primary GitHub email. You do NOT need cryptographic (e.g. gpg) signing.
* Use `git commit -s --amend ...` to add a signoff to the latest commit, if you forgot.

To automatically signoff on every commit, copy the `community/dco-signoff-hook/prepare-commit-msg` file to the `.git/hooks` directory in your repo or if you already have such a hook, merge the contents into your existing hook.

*Note*: Some projects will provide specific configuration to ensure all commits are signed-off. Please check the project's documentation for more details.

## Tests

Make sure your changes are properly covered by automated tests. We aim to build an efficient test suite that is low cost to maintain and bring value to project. Prefer writing unit-tests over heavy end-to-end (e2e) tests. However, sometimes e2e tests are necessary. If you aren't sure, ask one of the maintainers about the requirements for your pull-request.
