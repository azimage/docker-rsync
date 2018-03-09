Docker Image Packaging for Rsync
================================

[![Travis](https://img.shields.io/travis/alvistack/docker-rsync.svg)](https://travis-ci.org/alvistack/docker-rsync)
[![GitHub release](https://img.shields.io/github/release/alvistack/docker-rsync.svg)](https://github.com/alvistack/docker-rsync/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/docker-rsync.svg)](https://github.com/alvistack/docker-rsync/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/alvistack/docker-rsync.svg)](https://hub.docker.com/r/alvistack/docker-rsync/)

rsync is an open source utility that provides fast incremental file transfer. rsync is freely available under the GNU General Public License and is currently being maintained by Wayne Davison.

Learn more about Rsync: <https://rsync.samba.org/>

Overview
--------

This Docker container makes it easy to get an instance of Rsync up and running.

### Quick Start

Start Rsync:

    # Pull latest image
    docker pull alvistack/docker-rsync

    # Run as detach
    docker run \
        -itd \
        --rm \
        --name rsync \
        --volume /tmp/source:/source \
        --volume /tmp/target:/target \
        alvistack/docker-rsync \
        rsync -avP --delete /source/ /target

**Success**. Rsync will now backup the `/source` directory to `/target` directory and exit.

Versioning
----------

The `latest` tag matches the most recent version of this repository. Thus using `alvistack/docker-rsync:latest` or `alvistack/docker-rsync` will ensure you are running the most up to date version of this image.

License
-------

-   Code released under [Apache License 2.0](LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <https://twitter.com/hswong3i>
    -   <https://github.com/hswong3i>

