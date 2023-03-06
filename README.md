# Dotfiles

My dotfiles, managed with [chezmoi](https://github.com/twpayne/chezmoi).

## Installation

1. Install [chezmoi](https://www.chezmoi.io) binary to bootstrap without brew.
2. `chezmoi init vsimon`

## Notes

`chezmoi` is the only dependency for a one-touch install experience without
clunky hand-rolled install scripts.

`Homebrew` and its dependencies are installed first and packages are managed
through a `Brewfile`.

`ohmyzsh` is installed through an external archive and
plugins/themes are specified in the `.zshrc` file.

`tmux` plugins are managed
with the `tpm` git-repo and plugins specified in the `.tmux.conf` file.

Shell history is managed by `atuin`.

## Credits

In tending my dotfiles over the years, I’ve drawn inspiration from a few
different places. Thank you to all of the following:

- Tom Payne for [his dotfiles](https://github.com/twpayne/dotfiles) and
[chezmoi](https://github.com/twpayne/chezmoi)
- Zach Holman for [his dotfiles](https://github.com/holman/dotfiles)