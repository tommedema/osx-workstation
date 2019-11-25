# osx-workstation
Personal repo to version control my workstation configuration.

## Manual
- auto hide dock
- default web browser to chrome
- enable tap to click
- enable 3 finger drag
- increase trackpad speed
- enable firewall

## ToDo
- default directories: `projects`, `dumps`, `screenshots`
- change default screenshot directory
- update all libraries
- enable auto lock with password
- install whatsapp
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

## Git

### Aliases

- `cd ~/tooling`
- `curl -O https://raw.githubusercontent.com/GitAlias/gitalias/master/gitalias.txt`
- run:
```
cat <<EOT >> ~/.gitconfig
[include]
    path = ~/tooling/gitalias.txt
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

### IDE
- `brew cask install visual-studio-code`

### Media
- `brew cask install spotify`
- `brew cask install vlc`
- `brew cask install webtorrent`
