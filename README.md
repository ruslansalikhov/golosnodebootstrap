# golosnodebootstrap
Bootstrapping golos node script

## About

This script will clone last golos sources from github, build it and setup on your system.

## How to use script

To build and install last version of golos node you can use the script using cURL:

```sh
curl -o- -L https://github.com/ruslansalikhov/golosbootstrap/releases/download/0.1.10/golosbootstrap.sh | bash
```

or Wget:

```sh
wget -qO- https://github.com/ruslansalikhov/golosbootstrap/releases/download/0.1.10/golosbootstrap.sh | bash
```

or you can download script and run it manually.

If you want only build package - add "build_only" argument:

```sh
curl -o- -L https://github.com/ruslansalikhov/golosbootstrap/releases/download/0.1.10/golosbootstrap.sh | bash -s -- build_only
```

If you want build custom branch - export GOLOS_BRANCH variable:

```sh
curl -o- -L https://github.com/ruslansalikhov/golosbootstrap/releases/download/0.1.10/golosbootstrap.sh | env GOLOS_BRANCH=tags/v0.17.2 bash -s -- --witness
```

