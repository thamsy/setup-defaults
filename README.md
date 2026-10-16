# Setup Defaults

Content Page:

- Git
- asdf
- Golang

## Git

```
cp .gitconfig ~/.gitconfig
```

## oh-my-zsh

...

## vim

```
cp .vimrc ~/.vimrc
```

## asdf

Add to `.zshrc`

```
# ASDF
export PATH="${ASDF_DATA_DIR:-$HOME/.asdf}/shims:$PATH"
. ~/.asdf/plugins/golang/set-env.zsh
export GOROOT="$(asdf where golang)/go/"
export PATH="$PATH:$(go env GOPATH)/bin"
```

## Golang
