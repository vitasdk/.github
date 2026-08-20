<p align="center">
  <img src="https://avatars.githubusercontent.com/u/12992966?s=400&u=eb84b01bfd696fa0d148537189170c24b11e4138&v=4" alt="VitaSDK logo" width="160">
</p>

<h1 align="center">VitaSDK</h1>

<p align="center">
  Open-source SDK and toolchain for PlayStation Vita homebrew development.
</p>

<p align="center">
  <a href="https://vitasdk.org/">Website</a> ·
  <a href="https://docs.vitasdk.org/">API Documentation</a> ·
  <a href="https://github.com/vitasdk/samples">Samples</a> ·
  <a href="https://github.com/vitasdk/packages">Packages</a>
</p>

VitaSDK is an independent community project providing the compiler toolchain,
system headers, libraries, build tools, packages, and infrastructure used to
develop software for the PlayStation Vita.

VitaSDK is not affiliated with or endorsed by Sony Interactive Entertainment.

## Quick Start

Set the SDK location and add its tools to your `PATH`:

```sh
export VITASDK=/usr/local/vitasdk
export PATH=$VITASDK/bin:$PATH
```

Bootstrap VitaSDK using `vdpm`:

```sh
git clone https://github.com/vitasdk/vdpm
cd vdpm
./bootstrap-vitasdk.sh
```

Check the installation:

```sh
vdpm status
```

Then take a look at the [samples](https://github.com/vitasdk/samples) and the
[VitaSDK API documentation](https://docs.vitasdk.org/).

For platform-specific installation instructions, Docker, package management,
updates, and other documentation, see [vitasdk.org](https://vitasdk.org/).

## Core Repositories

- [`vita-toolchain`](https://github.com/vitasdk/vita-toolchain) — Vita ELF and SELF tooling
- [`vita-headers`](https://github.com/vitasdk/vita-headers) — PlayStation Vita system headers and NIDs
- [`newlib`](https://github.com/vitasdk/newlib) — Vita newlib port
- [`packages`](https://github.com/vitasdk/packages) — libraries and packages available for VitaSDK
- [`samples`](https://github.com/vitasdk/samples) — example Vita applications

## Tools

- [`vdpm`](https://github.com/vitasdk/vdpm) — VitaSDK package and installation management
- [`vita-makepkg`](https://github.com/vitasdk/vita-makepkg) — package building tools

## Project Infrastructure

Most users do not need these repositories directly, but they support VitaSDK
development, packaging, builds, and distribution.

- [`buildscripts`](https://github.com/vitasdk/buildscripts) — SDK build and release infrastructure
- [`vitasdk-autobuild`](https://github.com/vitasdk/vitasdk-autobuild) — automated package building
- [`docker`](https://github.com/vitasdk/docker) — container and build environments
- [`artifacts`](https://github.com/vitasdk/artifacts) — project build artifacts

## Contributing

Contributions are welcome.

Project-wide and other significant decisions use the RFC process defined in
[VitaSDK Governance](https://github.com/vitasdk/.github/blob/main/GOVERNANCE.md).

Bug reports, code, documentation, testing, reviews, and technical discussion
are all valuable ways to contribute.
