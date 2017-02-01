# GlassFish 3

GlassFish is an open-source application server project started by Sun Microsystems for the Java EE platform and now sponsored by Oracle Corporation. The supported version is called Oracle GlassFish Server. GlassFish is free software, dual-licensed under two free software licences: the Common Development and Distribution License (CDDL) and the GNU General Public License (GPL) with the classpath exception.

This repository provides Docker images for GlassFish 3.1.2.2 only. For GlassFish 4 images, see the official [glassfish](https://hub.docker.com/_/glassfish/) image (deprecated) or [glassfish/server](https://hub.docker.com/r/glassfish/server/).

## Starting GlassFish Server

```
$ docker run -d ucalgary/glassfish
```

This image calls `asadmin start-domain --verbose` to start the default GlassFish domain as its command. By specifying `--verbose`, the domain is started as a foreground process, with logs outputted to `stdout` and `stderr`. Stopping a running container will stop the Domain Adminisration Server (DAS).

## Maintenance

This image is currently maintained by the Research Management Systems project at the [University of Calgary](http://www.ucalgary.ca/).
