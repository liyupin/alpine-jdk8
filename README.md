alpine-jdk8
=============

This image is the jdk8 base. It comes from [alpine-monit][alpine-monit].

## Build

```
docker build -t rawmind/alpine-jdk8:<version> .
```

## Versions

- `1.8.112-2` [(Dockerfile)](https://github.com/rawmind0/alpine-jdk8/blob/1.8.112-2/Dockerfile)


## Usage

To use this image include `FROM rawmind/alpine-jdk8` at the top of your `Dockerfile`. Starting from `rawmind/alpine-monit` provides you with the ability to easily start any service using monit. monit will also keep it running for you, restarting it when it crashes.

To start your service using monit:

- create a monit conf file in `/opt/monit/etc/conf.d`
- create a service script that allow start, stop and restart function

[alpine-monit]: https://github.com/rawmind0/alpine-monit/
[jdk8]: http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html