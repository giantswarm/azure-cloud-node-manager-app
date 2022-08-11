# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project's packages adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.23.17-gs1] - 2022-08-11

### Changed

- Bump upstream image to 1.23.17.

## [1.1.17-gs1] - 2022-07-01

### Changed

- Bump upstream image to 1.1.17.

## [1.1.11-gs1] - 2022-04-13

### Changed

- Bumped to upstream version 1.1.11.

## [1.1.8-gs6] - 2022-03-23

### Changed

- Switch `dnsPolicy` to `Default` to allow running the pod when coreDNS is still not healthy.

## [1.1.8-gs5] - 2022-03-21

### Added

- Add VerticalPodAutoscaler CR.

## [1.1.8-gs4] - 2022-03-16

### Fixed

- Removed kubeconfig from flags to use inCluster.

## [1.1.8-gs3] - 2022-03-16

### Fixed

- Removed NodeSelector that was creating pods in the Master nodes only.

## [1.1.8-gs2] - 2022-03-16

### Changed

- Relax tolerations to make scheduling happen as soon as possible.
## [1.1.8-gs1] - 2022-03-14

[Unreleased]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.23.17-gs1...HEAD
[1.23.17-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.17-gs1...v1.23.17-gs1
[1.1.17-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.11-gs1...v1.1.17-gs1
[1.1.11-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs6...v1.1.11-gs1
[1.1.8-gs6]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs5...v1.1.8-gs6
[1.1.8-gs5]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs4...v1.1.8-gs5
[1.1.8-gs4]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs3...v1.1.8-gs4
[1.1.8-gs3]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs2...v1.1.8-gs3
[1.1.8-gs2]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs1...v1.1.8-gs2
[1.1.8-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v0.0.0...v1.1.8-gs1
