# swift-concurrency-extras-artifacts

Build-and-release automation for `swift-concurrency-extras` XCFramework
artifacts.

Upstream package:
`https://github.com/pointfreeco/swift-concurrency-extras`

Artifacts produced by this repository are consumed by:
`https://github.com/spm-binary/swift-concurrency-extras.git`

## Release Flow

Run the `Build release` workflow with:

- `upstream_ref`: upstream tag or branch to build, such as `1.3.2`
- `release_tag`: release tag to create in this repository, usually the same
  semantic version

The workflow builds `ConcurrencyExtras` as an XCFramework zip asset and uploads
a `checksums.txt` file containing the SwiftPM checksum.
