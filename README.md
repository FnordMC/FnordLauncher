# <img src="./program_info/gg.arson.FnordLauncher.svg" alt="Fnord Launcher logo" width="96"/> Fnord Launcher

Fnord Launcher is a **fork** of [Fjord Launcher](https://github.com/unmojang/FjordLauncher).

## Advantages of this fork over Fjord Launcher

- Does not require a Mojang account

## Having a problem with the launcher?

**Do not** open an issue in the Prism Launcher repo, and **do not** ask about Fnord Launcher in the Prism Launcher Discord server. Instead, ask in #fnord-launcher in our [Matrix space](https://matrix.to/#/#unmojang:matrix.org), or [open an issue](https://github.com/fnordmc/FnordLauncher/issues), in this repository.

## Installation

### Windows

You can get installers or portable builds from the [releases section](https://github.com/fnordmc/FnordLauncher/releases/latest), MSVC builds are recommended over MinGW builds, but there's no real difference.

### macOS

There are builds for macOS in the [releases section](https://github.com/fnordmc/FnordLauncher/releases/latest).

### Flatpak

```Shell
flatpak remote-add --user --if-not-exists unmojang https://fnord.github.io/fnord-flatpak/index.flatpakrepo
flatpak install org.unmojang.FjordLauncher
```

### Nix

This repository contains a Nix flake:

```Shell
nix run github:fnordmc/FnordLauncher
```

See [nix/README.md](nix/README.md) for details.

### Other Linux

AppImages are available in the [releases section](https://github.com/fnordmc/FnordLauncher/releases/latest).

## Building

To build the launcher yourself, follow the instructions on the Prism Launcher website, but clone this repo instead:

- [Windows](https://prismlauncher.org/wiki/development/build-instructions/windows/)
- [Linux](https://prismlauncher.org/wiki/development/build-instructions/linux/)
- [MacOS](https://prismlauncher.org/wiki/development/build-instructions/macos/)
- [OpenBSD](https://prismlauncher.org/wiki/development/build-instructions/openbsd/)

## Notes

- You can easily use a custom version of authlib-injector on an instance. Select the instance in the main window, click "Edit" (or Ctrl+I/Command+I), go to the Version tab, click "Add Agents", and select your authlib-injector JAR. If your JAR is not correctly identified as authlib-injector, make sure the `Agent-Class` field in the JAR's MANIFEST.MF is `moe.yushi.authlibinjector.Premain`.
