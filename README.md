# Just-based Copier template for Python
[![Copier](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/copier-org/copier/master/img/badge/badge-grayscale-border.json)](https://github.com/copier-org/copier)

## Usage

### Install

```shell
uv tool install --with jinja2-shell-extension --with jinja2-time copier
```

### Seed new project

```shell
uvx copier copy --trust --vcs-ref main gh:makukha/copier-python .
just init
just pre-merge
```

### Test template locally

```shell
uvx copier copy --trust --vcs-ref main . .tmp
cd .tmp
just init
just sync
just pre-merge
```
