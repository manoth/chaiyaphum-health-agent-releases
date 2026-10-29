# Chaiyaphum Health Agent Releases

Public, binary-only distribution repository for Health Agent installers and
automatic updates. The application source code remains in the private
`chaiyaphum-health-agent` repository.

Each release contains:

- Windows AMD64 executable and ZIP installer
- Linux AMD64 executable, DEB package, and tarball
- SHA-256 checksums
- an Ed25519-signed `release-manifest.json`

The release workflow reads source tags through a read-only deploy key, builds
the artifacts, signs the manifest, and publishes only the generated files.

Do not place source code, configuration secrets, certificates, or private keys
in this repository.
