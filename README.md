docker-oldgit [![Docker Build Status](https://img.shields.io/docker/build/iamdanfox/oldgit.svg)]()
=============

Dockerfile which builds git 1.7.1 from source on top of Centos 7.  Three layers, roughly 135 MB in total.

```
$ docker run iamdanfox/oldgit:latest git --version

latest: Pulling from iamdanfox/oldgit
d9aaf4d82f24: Pull complete
f1447c5ec907: Pull complete
e58f2bb8c2cf: Pull complete
Digest: sha256:930290808e5d5894192379b485dccb430e9bb4583c9243ab52bc01eb86c1b45b
Status: Downloaded newer image for iamdanfox/oldgit:latest
git version 1.7.1
```

Every tag and commit to develop is published using Docker Hub's "Automated Builds": https://hub.docker.com/r/iamdanfox/oldgit/.

## Why

I needed to run tests against git 1.7.1, but because it was released so long ago (April 2010), many package managers don't seem to have it anymore.
