# Dotfiles

My dotfiles, managed declaratively with [chezmoi](https://github.com/twpayne/chezmoi).

## Installation

1. Install [chezmoi](https://www.chezmoi.io) binary to bootstrap without `brew`.
2. `chezmoi init vsimon`

## Notes

`chezmoi` is the only dependency for a one-touch install experience without
clunky hand-rolled scripts.

`brew` and its dependencies are installed first and packages are managed through
a [`Brewfile`](Brewfile).

`ohmyzsh` is installed through an external archive and plugins/themes are
specified in the [`.zshrc`](dot_zshrc) file.

`tmux` plugins are managed with the `tpm` git-repo and plugins are specified in
the [`.tmux.conf`](dot_tmux.conf) file.

`git` configuration is templated with the [`.chezmoi.yaml.tmpl`](.chezmoi.yaml.tmpl) file.

Shell history is managed by `atuin`.

## How to create and update an age file

Update somefile and reencrypt the file with:

```sh
age --encrypt -r [public-key] --armor ~/.somefolder/somefile > private_dot_somefolder/encrypted_somefile.age
```

The public key is listed in `.config/age/key`.

## Credits

In tending my dotfiles over the years, I’ve drawn inspiration from a few
different places. Thank you to all of the following:

- Tom Payne for [his dotfiles](https://github.com/twpayne/dotfiles) and
[chezmoi](https://github.com/twpayne/chezmoi)
- Zach Holman for [his dotfiles](https://github.com/holman/dotfiles)
