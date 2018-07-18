# osx-workstation
Personal repo to version control my workstation configuration.

## Dev Tooling

### Homebrew
- `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

### Yarn and Node.js
- `brew install yarn`

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

You can now use aliases like:
- `git put "my commit message"` to commit all and push.
- `git s` for git status
