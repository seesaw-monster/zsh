# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a personal zsh configuration repository that provides shell customization, aliases, and plugin management using zplug. The main configuration file is `myzshrc` which is sourced from the user's main `.zshrc` file.

## Key Components

- **myzshrc**: Main zsh configuration file containing aliases, functions, and plugin setup
- **README.md**: Installation and setup instructions in Japanese

## Common Development Tasks

When making changes to zsh configuration:
- Test changes by sourcing the configuration: `source ~/.config/zsh/myzshrc`
- Reload the full shell configuration: `source ~/.zshrc`
- Check plugin status: `zplug status`
- Install new plugins: `zplug install`

## Git Operations

Use English for all git commit messages, pull requests, and branch names as specified in the user's global instructions.

## Architecture Notes

The configuration uses:
- **zplug** for plugin management
- **peco** for interactive command history and directory navigation
- **fzf** for fuzzy finding
- **powerlevel10k** theme for prompt customization

Key keybindings:
- `Ctrl+R`: Command history search with peco
- `Ctrl+X`: Directory navigation with peco
- `Ctrl+L`: Accept autosuggestion

## Custom Functions

- `mkcd()`: Create directory and navigate to it
- `taikin()`: Calculate work end time (adds 8h 30m to input time)
- `test-case()`: AtCoder testing function
- `teisyutu()`: AtCoder submission function