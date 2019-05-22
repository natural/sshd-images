# sshd images

These images are used for testing.

This repo contains Dockerfiles for various OS images, all with `sshd`
running as the entry point.


## Installation

Local install if necessary:

```sh
$ ./images-build
```


## Push

Remote image push:
```sh
$ ./images-build && ./images-push
```
