# <img src="./program_info/xyz.fnordmc.FnordLauncher.svg" alt="Fnord Launcher logo" width="96"/> Fnord Launcher

Fnord Launcher is a **fork** of [Fjord Launcher](https://github.com/unmojang/FjordLauncher).

## Advantages of this fork over Fjord Launcher

- Does not require a Microsoft account

## Values

Refer to [VALUES.md](VALUES.md)

## Having a problem with the launcher?

**Do not** open an issue in the Prism Launcher repo, and **do not** ask about Fnord Launcher in the Prism Launcher Discord server. Instead, ask in #fnordlauncher on libera.chat, or [open an issue](https://github.com/fnordmc/FnordLauncher/issues), in this repository.

## Installation

### Flatpak

You can install the FnordLauncher flatpak with these commands:

```Shell
flatpak remote-add --if-not-exists FnordMC https://fnordmc.github.io/Fnord-launcher-flatpak/fnord.flatpakrepo
flatpak install xyz.fnordmc.FnordLauncher
```

### Windows

You can get installers or portable builds from the [releases section](https://github.com/fnordmc/FnordLauncher/releases/latest), MSVC builds are recommended over MinGW builds, but there's no real difference.

### macOS

There are builds for macOS in the [releases section](https://github.com/fnordmc/FnordLauncher/releases/latest).

### Nix

This repository contains a Nix flake:

```Shell
nix run github:fnordmc/FnordLauncher
```

See [nix/README.md](nix/README.md) for details.

### Other Linux

AppImages are available in the [releases section](https://github.com/fnordmc/FnordLauncher/releases/latest).

## Building

To build the launcher yourself, follow the [instructions on the Prism Launcher website](https://prismlauncher.org/wiki/development/build-instructions), but clone this repo instead.

## Notes

- You can easily use a custom version of Loki or authlib-injector on an instance. Select the instance in the main window, go to the Version tab, delete any Yggdrasil Agents if present, click "Add Agents", and select your Yggdrasil Agent JAR. If your JAR is not correctly identified, make sure the `Agent-Class` or `Premain-Class` field in the JAR's MANIFEST.MF matches either `moe.yushi.authlibinjector.Premain` or `org.unmojang.loki.Loki`.
