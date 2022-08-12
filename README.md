# Simon's Working Environment

This repo contains links and config files for Simon's typical working environment

## Command Line Tools

### [Homebrew](https://brew.sh/)
Essential package manager for macOS

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

### [Fish Shell](https://fishshell.com/)
A smart and user-friendly command line shell

`brew install fish`

### [Oh My Fish](https://github.com/oh-my-fish/oh-my-fish)
Easily install packages for Fish Shell

`curl https://raw.githubusercontent.com/oh-my-fish/oh-my-fish/master/bin/install | fish`

### [bobthefish Theme](https://github.com/oh-my-fish/theme-bobthefish)
A Powerline-style Git-aware fish theme optimized for awesome

`omf install bobthefish`

Install a [nerd fonts patched font](https://github.com/ryanoasis/nerd-fonts#option-4-homebrew-fonts), and enable nerd fonts support:

```shell
brew tap homebrew/cask-fonts
brew install --cask font-hack-nerd-font
set -g theme_nerd_fonts yes
```

### [Oh My Fish brew](https://github.com/oh-my-fish/plugin-brew)
Oh My Fish plugin to integrate Homebrew paths into shell

`omf install brew`

### [Oh My Fish cd](https://github.com/oh-my-fish/plugin-cd)
Oh My Fish plugin providing a new `cd` command to help you change the current working directory fast.

`omf install cd`

### [Oh My Fish git aliases](https://github.com/jhillyerd/plugin-git)
Creates some great shorthand aliases for common git calls

`omf install https://github.com/jhillyerd/plugin-git`

### [Oh My Fish osx](https://github.com/oh-my-fish/plugin-osx)
A number of handy functions for use in macOS

`omf install osx`

### [Oh My Fish hash](https://github.com/oh-my-fish/plugin-hash)
Computes string digests using various hashing algorithms

`omf install hash`

### Git
macOS comes with an outdated version of the Git CLI. Install the latest with 

`brew install git`

### Go
Install the latest version with

`brew install go`

### [golangci-lint](https://golangci-lint.run/)
A fast linters runner for Go

`brew install golangci-lint`

### [gotestsum](https://github.com/gotestyourself/gotestsum)
`gotestsum` runs tests using `go test -json`, prints formatted test output, and a summary of the test run. It is designed to work well for both local development, and for automation like CI.

### [colima](https://github.com/abiosoft/colima)
Container runtimes for macOS - great alternative to Docker Desktop

```shell
brew install colima
brew install docker docker-compose
mkdir -p ~/.docker/cli-plugins
ln -sfn /opt/homebrew/opt/docker-compose/bin/docker-compose ~/.docker/cli-plugins/docker-compose

colima start
```

---

## Mac Apps

### [iTerm2](https://iterm2.com/)
Great terminal emulator for macOS

### [Alfred](https://www.alfredapp.com/)
A productivity application for macOS.

- Launch applications and find files on your mac using hotkeys
- Clipboard history
- Snippets
- Perform quick maths calculations

### [Display Maid](https://funk-isoft.com/display-maid.html)
Save and restore windows based on your display configuration or user created profiles

### [IntelliJ IDEA Ultimate](https://www.jetbrains.com/idea/)
My IDE of choice. Includes great support for Go. Recommend the following plugins:

| Plugin | Description                                                |
| --- |------------------------------------------------------------|
| Go | Adds Go support (this has all the functionality of GoLand) |
| GO Imports Tidy | Helps group your Go import lines |
| Go Linter | Integrates the golangci-lint linters |


---

## Config files
This repo contains the following config files:

| Filename | Description                                                 |
| -------- |-------------------------------------------------------------|
| iTerm-profile.json | Config file for iTerm2. Import under Preferences > Profiles |
