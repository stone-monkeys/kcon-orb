# Kconnect Orb for CircleCI

[![CircleCI Build Status](https://circleci.com/gh/stone-monkeys/kcon-orb.svg?style=shield "CircleCI Build Status")](https://circleci.com/gh/stone-monkeys/kcon-orb) [![CircleCI Orb Version](https://badges.circleci.com/orbs/db-cci-ns/k-connect.svg)](https://circleci.com/orbs/registry/orb/db-cci-ns/k-connect) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/stone-monkeys/kcon-orb/master/LICENSE) [![CircleCI Community](https://img.shields.io/badge/community-CircleCI%20Discuss-343434.svg)](https://discuss.circleci.com/c/ecosystem/orbs)



This orb allows users to install and utilizes kconnects

## Commands

| Commands          | Meaning                                                           | Defaults |
|-------------------|-------------------------------------------------------------------|----------|
| install           | This command installs kconnect to your execution environment      | N/A      |
| configure         | File or remote location to use to set the default configuration   | N/A      |
| use               | Connect to a Kubernetes cluster provider and cluster              | N/A      |
| to                | Reconnect to a connection history entry                           | N/A      |
| version           | Display version & build information                               | N/A      |
| ls                | Query the user’s connection history                               | N/A      |


## How to Utilize this Orb

Here are some rough steps to get started with this orb:

[CircleCI Example] (https://github.com/stone-monkeys/kcon-orb/blob/main/src/examples/example.yml)

## Resources

[CircleCI Orb Registry Page](https://circleci.com/orbs/registry/orb/db-cci-ns/kcon-orb) - The official registry page of this orb for all versions, executors, commands, and jobs described.
[CircleCI Orb Docs](https://circleci.com/docs/2.0/orb-intro/#section=configuration) - Docs for using and creating CircleCI Orbs.

### How to Contribute

We welcome [issues](https://github.com/stone-monkeys/kcon-orb/issues) to and [pull requests](https://github.com/stone-monkeys/kcon-orb/pulls) against this repository!

### How to Publish
* Create and push a branch with your new features.
* When ready to publish a new production version, create a Pull Request from _feature branch_ to `master`.
* The title of the pull request must contain a special semver tag: `[semver:<segment>]` where `<segment>` is replaced by one of the following values.

| Increment | Description|
| ----------| -----------|
| major     | Issue a 1.0.0 incremented release|
| minor     | Issue a x.1.0 incremented release|
| patch     | Issue a x.x.1 incremented release|
| skip      | Do not issue a release|

Example: `[semver:major]`

* Squash and merge. Ensure the semver tag is preserved and entered as a part of the commit message.
* On merge, after manual approval, the orb will automatically be published to the Orb Registry.


For further questions/comments about this or other orbs, visit the Orb Category of [CircleCI Discuss](https://discuss.circleci.com/c/orbs).

