# <img src="./program_info/gg.arson.FnordLauncher.svg" alt="Fnord Launcher logo" width="96"/> Fnord Launcher

Fnord Launcher is a **fork** of [Fjord Launcher](https://github.com/unmojang/FjordLauncher).

## Advantages of this fork over Fjord Launcher

- Does not require a Mojang account

## Having a problem with the launcher?

<<<<<<< HEAD
**Do not** open an issue in the Prism Launcher repo, and **do not** ask about Fnord Launcher in the Prism Launcher Discord server. Instead, ask in #fnordlauncher on libera.chat, or [open an issue](https://github.com/fnordmc/FnordLauncher/issues), in this repository.
=======
**Do not** open an issue in the Prism Launcher repo, and **do not** ask about Fjord Launcher in the Prism Launcher Discord server. Instead, ask in #fjord-launcher in our [Matrix space](https://matrix.to/#/#unmojang:matrix.org), or [open an issue](https://github.com/unmojang/FjordLauncher/issues), in this repository.
>>>>>>> upstream/HEAD

## Installation

### Windows

You can get installers or portable builds from the [releases section](https://github.com/fnordmc/FnordLauncher/releases/latest), MSVC builds are recommended over MinGW builds, but there's no real difference.

### macOS

<<<<<<< HEAD
There are builds for macOS in the [releases section](https://github.com/fnordmc/FnordLauncher/releases/latest).
=======
#### [Homebrew](https://brew.sh) (recommended)

```Shell
brew tap unmojang/homebrew-unmojang
brew install --cask fjordlauncher
```

#### macOS (Manual)

There are builds for macOS in the [releases section](https://github.com/unmojang/FjordLauncher/releases/latest).

### Flatpak

```Shell
flatpak remote-add --user --if-not-exists unmojang https://unmojang.github.io/unmojang-flatpak/index.flatpakrepo
flatpak install org.kde.Platform/x86_64/6.10
flatpak install org.unmojang.FjordLauncher
```

### Arch Linux

Fjord Launcher is [available](https://aur.archlinux.org/packages?O=0&K=fjordlauncher) from the AUR:

```Shell
paru -S fjordlauncher
paru -S fjordlauncher-git # build latest Git commit from source
```

`fjordlauncher` is available in [Chaotic-AUR](https://aur.chaotic.cx/).

The `fjordlauncher-bin` AUR package is broken; see [https://github.com/unmojang/FjordLauncher/issues/20](https://github.com/unmojang/FjordLauncher/issues/20).

### Debian/Ubuntu

Install from the MPR with [Mist](https://docs.makedeb.org/using-the-mpr/mist-the-mpr-cli/#installing-mist):

```Shell
mist install fjordlauncher
mist install fjordlauncher-git # build latest Git commit from source
```
>>>>>>> upstream/HEAD

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

- You can easily use a custom version of authlib-injector on an instance. Select the instance in the main window, click "Edit" (or Ctrl+I/Command+I), go to the Version tab, click "Add Agents", and select your authlib-injector JAR. If your JAR is not correctly identified as authlib-injector, make sure the `Agent-Class` field in the JAR's MANIFEST.MF is `moe.yushi.authlibinjector.Premain`.
