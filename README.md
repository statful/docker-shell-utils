# Shell Utils docker image

# What is shell utils?

> Shell utils are utilities that sometimes are required fro scripting certain actions.

At the moment this image contains:
* envsubst
* gettext

# TL;DR;

```bash
docker run -ti --rm statful/shell-utils /bin/bash
```

# Supported tags and respective `Dockerfile` links

* [`latest` (Dockerfile)](https://github.com/statful/docker-shell-utils/blob/master/Dockerfile)

Subscribe to project updates by watching the [statful/docker-shell-utils GitHub repo](https://github.com/statful/docker-shell-utils).

# Get this image

The recommended way to get the Statful shell-utils Docker Image is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/r/statful/shell-utils).

```bash
docker pull statful/shell-utils:latest
```

To use a specific version, you can pull a versioned tag. You can view the [list of available versions](https://hub.docker.com/r/statful/shell-utils/tags/) in the Docker Hub Registry.

```bash
docker pull statful/shell-utils:[TAG]
```

If you wish, you can also build the image yourself.

```bash
# Building the latest image
docker build -t statful/shell-utils:latest 'https://github.com/statful/docker-shell-utils.git/tree/latest'

# Building a specific tag, e.g., 1.16
docker build -t statful/shell-utils:1.16 'https://github.com/statful/docker-shell-utils.git/tree/1.16'
```

# Configuration

## Running commands

To run commands inside this container you can use `docker run`, for example to execute `envsubst` you can follow the example below:

```bash
docker run foo --rm --name shell-utils statful/shell-utils:latest -- envsubst
```

### Environment variables

```bash
docker run -ti -e 'FOO=BAR' -e 'FOO2=BAR2' --rm statful/shell-utils -- envsubst
```

# Contributing

We'd love for you to contribute to this container. You can request new features by creating an [issue](https://github.com/statful/docker-shell-utils/issues), or submit a [pull request](https://github.com/statful/docker-shell-utils/pulls) with your contribution.

# Issues

If you encountered a problem running this container, you can file an [issue](https://github.com/statful/docker-shell-utils/issues). For us to provide better support, be sure to include the following information in your issue:

- Host OS and version
- Docker version (`docker version`)
- Output of `docker info`
- Version of this container
- The command you used to run the container, and any relevant output you saw (masking any sensitive information)

# License

Copyright (c) 2019 Statful. All rights reserved.

This work is licensed under the terms of the MIT license.
For a copy, see <https://opensource.org/licenses/MIT>.

