# osx-workstation
Personal repo to version control my workstation configuration.

## ToDo
- enable tap to click
- enable 3 finger drag
- auto hide dock
- create more screen space in screen settings
- default web browser to chrome
- always show hidden files in finder
- default directories: `projects`, `dumps`, `screenshots`
- change default screenshot directory
- update all libraries
- enable firewall
- enable encryption (firevault)
- enable auto lock with password
- install whatsapp
- install hyper
- install google keep

## Dev Tooling

### Homebrew
- `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

### Yarn and Node.js (with nvm)
- `curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash`
- `nvm install lts/carbon`
- `brew install yarn --without-node`

## Bash scripts

### mkcd: Create and move into directory

```
cat <<EOT >> ~/.bashrc

mkcd () {
  mkdir "$1"
  cd $_
}
EOT
```
  

## Init

- `mkcd ~/workstation`

## Git

### Aliases

- `cd ~/workstation`
- `curl -O https://raw.githubusercontent.com/GitAlias/gitalias/master/gitalias.txt`
- run:
```
cat <<EOT >> ~/.gitconfig
[include]
    path = ~/workstation/gitalias.txt
EOT
```

Modify gitalias.txt to include:

```
puta = !git add -A  && git put
```

You can now use aliases like:
- `git put "my commit message"` to commit all and push
- `git puta "this adds all files incl untracked ones and commit"`
- `git s` for git status

## Apps

### Tools
- `brew cask install caffeine`

### IDE
- `brew cask install visual-studio-code`

### Terminal
- `brew cask install hyper`

### Browser
- `brew cask install google-chrome`

### Design
- `brew cask install sketch`

### Media
- `brew cask install spotify`
- `brew cask install vlc`
- `brew cask install webtorrent`
