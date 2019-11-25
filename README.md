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
- `touch ~/.zshrc`
- `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash`
- `nvm ls-remote`
- `nvm install lts/dubnium`
- `curl -o- -L https://yarnpkg.com/install.sh | bash`

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

### Browser
- `brew cask install google-chrome`

### Tools
- `brew cask install caffeine`

### IDE
- `brew cask install visual-studio-code`

### Media
- `brew cask install spotify`
- `brew cask install vlc`
- `brew cask install webtorrent`
