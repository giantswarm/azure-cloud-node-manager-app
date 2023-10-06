# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project's packages adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Add `global.podSecurityStandards.enforced` value for PSS migration.

### Fixed

- Added required exceptions for PSS.

## [1.24.18-gs3] - 2023-05-10

### Changed

- Remove `capabitlities.apiversion.has` check for VPA to avoid race condition between this app being installed and the api-version providing app being installed
  - With this change the installation of the chart will fail until the `api-version` is available

## [1.24.18-gs2] - 2023-05-09

### Changed

- Upgrade `Chart.yaml` `apiVersion` from `v1` to `v2`
  - this is required to get `capabilities` conditional to work with `HelmReleases` 
  
## [1.24.18-gs1] - 2023-05-03

### Changed

- Disable PSPs for k8s 1.25 and newer.
- Bump to upstream version 1.24.18.

## [1.24.6-gs1] - 2022-12-21

- Fix resources in yaml. it was defined twice

## [1.24.5-gs1] - 2022-09-14

### Changed

- Bump upstream image to 1.24.5.

## [1.23.17-gs2] - 2022-08-23

### Changed

- Push to default catalog.
 
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

[Unreleased]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.24.18-gs3...HEAD
[1.24.18-gs3]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.24.18-gs2...v1.24.18-gs3
[1.24.18-gs2]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.24.18-gs1...v1.24.18-gs2
[1.24.18-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.24.6-gs1...v1.24.18-gs1
[1.24.6-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.24.5-gs1...v1.24.6-gs1
[1.24.5-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.23.17-gs2...v1.24.5-gs1
[1.23.17-gs2]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.23.17-gs1...v1.23.17-gs2
[1.23.17-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.17-gs1...v1.23.17-gs1
[1.1.17-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.11-gs1...v1.1.17-gs1
[1.1.11-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs6...v1.1.11-gs1
[1.1.8-gs6]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs5...v1.1.8-gs6
[1.1.8-gs5]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs4...v1.1.8-gs5
[1.1.8-gs4]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs3...v1.1.8-gs4
[1.1.8-gs3]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs2...v1.1.8-gs3
[1.1.8-gs2]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v1.1.8-gs1...v1.1.8-gs2
[1.1.8-gs1]: https://github.com/giantswarm/azure-cloud-node-manager-app/compare/v0.0.0...v1.1.8-gs1
