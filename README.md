# My i3 Dotfiles

My personal Linux desktop configuration files, featuring the **i3 Window Manager** and **Fish Shell**.

A lightweight, keyboard-driven environment customized for productivity, development, and everyday Linux usage.

## Overview

This repository contains my personal dotfiles for configuring and customizing my Linux desktop environment.

I use i3 as my tiling window manager and Fish as my interactive shell, focusing on a minimal, efficient workflow with keyboard-driven navigation.

The repository also serves as a backup of my configurations, making it easier to reproduce my setup on another Linux installation.

## Components

| Component | Description |
|---|---|
| **i3** | Lightweight tiling window manager for X11 |
| **Fish** | Interactive command-line shell with autosuggestions and syntax highlighting |

### i3 Window Manager

[i3](https://i3wm.org/) is a tiling window manager designed for efficient window management and keyboard-based navigation.

It offers:

- Automatic window tiling
- Configurable keyboard shortcuts
- Multiple workspaces
- Lightweight resource usage
- Customizable window layouts

### Fish Shell

[Fish](https://fishshell.com/) is a modern interactive shell designed for usability and productivity.

It provides:

- Command-line autosuggestions
- Syntax highlighting
- Tab completion
- Customizable prompts
- Shell functions and aliases

## Repository Structure

```text
My-i3-dotfiles/
├── i3/           # i3 window manager configuration
├── fish/         # Fish shell configuration
└── README.md     # Documentation
```

## Installation

### Requirements

- Linux
- X11
- i3 Window Manager
- Fish Shell
- Git

### 1. Install Dependencies

For Fedora:

```bash
sudo dnf install i3 fish git
```

For Arch Linux:

```bash
sudo pacman -S i3-wm fish git
```

For Debian/Ubuntu:

```bash
sudo apt install i3 fish git
```

### 2. Clone the Repository

```bash
git clone https://github.com/Fai707/My-i3-dotfiles.git
cd My-i3-dotfiles
```

### 3. Back Up Existing Configurations

Before installing, back up your current configurations:

```bash
cp -a ~/.config/i3 ~/.config/i3.backup
cp -a ~/.config/fish ~/.config/fish.backup
```

Run each command only if its corresponding configuration directory exists.

### 4. Install the Dotfiles

Copy the configurations into your local `.config` directory:

```bash
mkdir -p ~/.config

cp -r i3 ~/.config/
cp -r fish ~/.config/
```

**Note:** These commands may overwrite files with matching names. Review the configurations and back up your existing files before copying.

### 5. Apply Changes

Reload i3 using:

```bash
i3-msg reload
```

Start a new Fish session:

```bash
fish
```

Some configuration changes may require restarting i3 or logging out and back in.

## Customization

These dotfiles reflect my personal workflow and may require adjustments for different systems.

You can modify the configurations to suit your preferences.

**i3 configuration:**

```text
~/.config/i3/
```

**Fish configuration:**

```text
~/.config/fish/
```

Before using these dotfiles, review any application paths, startup commands, keybindings, and system-specific settings.

## Why i3?

I prefer a lightweight, keyboard-driven desktop environment that gives me more control over how I interact with my system.

Using i3 allows me to:

- Navigate efficiently between applications.
- Organize windows across multiple workspaces.
- Minimize unnecessary desktop overhead.
- Customize my development environment.
- Learn more about Linux desktop configuration.

## Goals

This repository serves several purposes:

- Maintain a backup of my Linux configurations.
- Make it easier to reproduce my desktop environment.
- Track configuration changes with Git.
- Share my setup with other Linux users.
- Continue experimenting with Linux customization.

## Resources

- [i3 Documentation](https://i3wm.org/docs/)
- [Fish Shell Documentation](https://fishshell.com/docs/current/)
- [ArchWiki – i3](https://wiki.archlinux.org/title/I3)

## Author

**Fai707**

GitHub: [github.com/Fai707](https://github.com/Fai707)
