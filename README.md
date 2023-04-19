# galaxy-debug

## What is it

`galaxy-debug` allows you to debug Ansible Galaxy roles using GitHub Actions workflows on the localhost.

## How to install

```
curl https://raw.githubusercontent.com/noobient/galaxy-debug/main/galaxy-debug -o "${HOME}/.local/bin/galaxy-debug"
```

You might have to restart your terminal emulator, before it appears in your PATH.

You also have to install **Podman** or **Docker**. Podman is recommended, as Docker will occasionally set wrong ownership on files under `/run/user`.

## How to use

For an example, please see:

[example_role](https://github.com/noobient/ansible-galaxy-example_role)

Enter the role root, then simply issue the `galaxy-debug` command.

By default, `galaxy-debug` uses Fedora 37 as its platform. If you want to override this, use the `--platform` parameter.
For a list of supported platforms, please see:

[bviktor @ Docker Hub](https://hub.docker.com/u/bviktor)

Except for `--platform`, all arguments will be passed onto Ansible, so you can pass Ansible arguments like `-v`, `-e`, etc.
