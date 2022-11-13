AppBundler Maven Build
======================
[![Build Status](https://travis-ci.com/evolvedbinary/appbundler-maven-build.svg?branch=main)](https://travis-ci.com/evolvedbinary/appbundler-maven-build)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.evolvedbinary.appbundler/appbundler/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.evolvedbinary.appbundler/appbundler)

This project simply downloads the latest AppBundler code from https://github.com/TheInfiniteKind/appbundler
and builds a Maven artifact `com.evolvedbinary.appbundler:appbundler`.

To build you will need a macOS machine with Git and Maven 3.6.0+ installed. You can then run:
```bash
$ git clone https://github.com/adamretter/appbundler-maven-build.git
$ cd appbundler-maven-build
$ mvn clean package
```
