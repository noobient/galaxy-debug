# galaxy-debug

## What is it

`ansible-debug` allows you to debug Ansible Galaxy roles using GitHub Actions workflows on the localhost.

## How to use

For an example, please see:

[example_role](https://github.com/noobient/ansible-galaxy-example_role)

Enter the role root, then simply issue the `galaxy-debug` command.

By default, `galaxy-debug` uses Fedora 37 as its platform. If you want to override this, use the `--platform` parameter.
For a list of supported platforms, please see:

[bviktor @ Docker Hub](https://hub.docker.com/repositories/bviktor)

Except for `--platform`, all arguments will be passed onto Ansible, so you can pass Ansible arguments like `-v`, `-e`, etc.
