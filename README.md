
## BOB - Bash On Board!

<img alt="bob" align="left" src="https://github.com/262life/artwork/raw/main/logos/BobLogo-Color.png" width="20%" height="20%">

Bash on Board! (we like to call it BoB!) is an open source **general purpose container** for Kubernetes, providing the utilities, support tools and a framework that allows a diverse set of problems to be solved for pod initialization and support to natively work with cloud-native environments.

![Hex.pm](https://img.shields.io/hexpm/l/apa)
[![CodeFactor](https://www.codefactor.io/repository/github/262life/bob/badge)](https://www.codefactor.io/repository/github/262life/bob)
![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/262life/bob/release/v0.9.13-RC1?label=build%20v0.9.13-RC1)
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/262life/bob)\
![Docker Pulls](https://img.shields.io/docker/pulls/262life/bob-core?label=docker%20pulls%20-%20bob-core)
![Docker Pulls](https://img.shields.io/docker/pulls/262life/bob-lowcarb?label=docker%20pulls%20-%20bob-lowcarb)
[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/262life/bob)\
[![Develop on Okteto](https://img.shields.io/badge/Okteto-Kubernetes%20for%20Developers-brightgreen?logo=apache-echarts)](https://cloud.okteto.com/deploy)
![Twitter Follow](https://img.shields.io/twitter/follow/262life?style=social)

BoB! turns a simple container instanciation into a power support tool for general troubleshooting, service rendering, and performance evaluation.  It does this by creating a core set services that house and manage the utilities as well as a super lightweight container to invoke in a pod.

BoB! integrates deeply into cloud native environments leveraging extension points and providing a seamless experience.
For more details about the solutions currently supported by BoB!, please refer to the [project status section](#project-status) below.
We plan to continue adding support for many common functions required based on community demand and engagement in future releases. See our [roadmap](docs/road.md) for more details.

## Licensing

BoB! is under the Apache 2.0 [License.](LICENSE.md)

## Getting Started and Documentation

For installation, deployment, and administration, see our [Documentation](docs/documentation.md)

## Contributing

We welcome contributions. 
* See the [Contributing](docs/contrib.md) regarding how to engage 
* See the [Getting Started](docs/getting_started.md) guide to setup your environment.

## Report a Bug

For filing bugs, suggesting improvements, or requesting new features, please open an [issue](https://github.com/262life/bob/issues).

## Contact

Please use the following to reach members of the community:

- Email: [bob@262.life](mailto:bob@262.life)

## Security

### Reporting Security Vulnerabilities

If you find a vulnerability or a potential vulnerability in BoB! please let us know immediately at [bob@262.life](mailto:bob@262.life). We'll send a confirmation email to acknowledge your
report, and we'll send an additional email when we've identified the issues positively or
negatively.

## Project Status

The status of each utility provider supported by BoB! can be found in the table below.

- **Alpha:** The API may change in incompatible ways in a later software release without notice, recommended for use only in short-lived testing clusters, due to increased risk of bugs and lack of long-term support.<br><br>
- **Beta:** Support for the overall features will not be dropped, though details may change. Support for upgrading or migrating between versions will be provided, either through automation or manual steps.<br><br>
- **Stable:** Features will appear in released software for many subsequent versions and support for upgrading between versions will be provided with software automation in the vast majority of scenarios.

|Name|Details|Status                              
| -  | - | - |
|core|The framework for the common utilities|Stable|                                           
|lowcarb|Lightweight container|Stable|            

### Official Releases

Official releases of BoB! can be found on the [releases page](https://github.com/262life/bob/releases).
Please note that it is **strongly recommended** that you use [official releases](https://github.com/262life/bob/releases) of BoB!, as unreleased versions from the master branch are subject to changes and incompatibilities that will not be supported in the official releases.
Builds from the master branch can have functionality changed and even removed at any time without compatibility support and without prior notice.


