# osx-workstation
Personal repo to version control my workstation configuration.

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

- `curl -O https://raw.githubusercontent.com/GitAlias/gitalias/master/gitalias.txt`
- run:
```
cat <<EOT >> ~/.gitconfig
[include]
    path = gitalias.txt
EOT
```

You can now use aliases like `git put description` to commit all and push.