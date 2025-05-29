
# C++ (cpp-cross)

Cross-platform development of C++ applications in Linux Sandbox

## Options

| Options Id | Description | Type | Default Value |
|-----|-----|-----|-----|
| imageVersion | Version of the container. | string | 0.1.0 |
| imageVariant | Base environment version. | string | debian-12 |
| tooling | Combination of tools, ie {vCMake}-{LLVM}-{LLVM-MINGW} | string | none |

## Image

This template references an image that was pre-built.

Image: [ghcr.io/darthkurt/devcontainer-cpp](https://github.com/DarthKurt/devcontainers/tree/main/src/devcontainer-cpp)

## Tooling

Pre-build versions. `none` means `none-none-none`.

| CMake Version | LLVM Version | LLVM MinGW Version |
|---------------|--------------|--------------------|
| 4.0.2         | none         | none               |
| none          | 19           | none               |
| none          | none         | 20250528           |
| 4.0.2         | 19           | none               |
| 4.0.2         | none         | 20250528           |
| none          | 19           | 20250528           |
| 4.0.2         | 19           | 20250528           |

## Using Vcpkg

This dev container and its associated image includes a clone of the [`Vcpkg`](https://github.com/microsoft/vcpkg) repo for library packages, and a bootstrapped instance of the [Vcpkg-tool](https://github.com/microsoft/vcpkg-tool) itself.

Most additional library packages installed using Vcpkg will be downloaded from their [official distribution locations](https://github.com/microsoft/vcpkg#security). To configure Vcpkg in this container to access an alternate registry, more information can be found here: [Registries: Bring your own libraries to vcpkg](https://devblogs.microsoft.com/cppblog/registries-bring-your-own-libraries-to-vcpkg/).

> Note: Please review the [Vcpkg license details](https://github.com/microsoft/vcpkg#license) to better understand its own license and additional license information pertaining to library packages and supported ports.


---

_Note: This file was auto-generated from the [devcontainer-template.json](https://github.com/DarthKurt/devcontainers-templates/blob/main/src/cpp-cross/devcontainer-template.json).  Add additional notes to a `NOTES.md`._
