AppBundler Maven Build
======================

This project simply downloads the latest AppBundler code from https://github.com/TheInfiniteKind/appbundler
and builds a Maven artifact `com.evolvedbinary.appbundler:appbundler`.

To build you will need a macOS machine with Mercurial 5.0.0+ and Maven 3.6.0+ installed. You can then run:
```bash
$ git clone https://github.com/adamretter/appbundler-maven-build.git
$ cd appbundler-maven-build
$ mvn clean package
```
