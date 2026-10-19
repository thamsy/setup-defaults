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

https://github.com/thamsy/optea-server/commit/ad8998ae147be64bd802644be4ff088614d6515f

For golang web server new instance, with:

- Postgres DB
- DB Migration
- Integration testing
- Web Server Framework
- Prod Deployment

When using, copy the entire repository and replace the references to `optea` with the new project name.
