AppBundler Maven Build
======================
[![Build Status](https://github.com/evolvedbinary/appbundler-maven-build/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/evolvedbinary/appbundler-maven-build/actions/workflows/ci.yml)
[![Maven Central](https://img.shields.io/maven-central/v/com.evolvedbinary.appbundler/appbundler?logo=apachemaven&label=maven+central&color=green)](https://central.sonatype.com/search?namespace=com.evolvedbinary.appbundler)

This project simply downloads the latest AppBundler code from https://github.com/evolvedbinary/appbundler or https://github.com/TheInfiniteKind/appbundler
and builds a Maven artifact `com.evolvedbinary.appbundler:appbundler`.

## Usage

To use the AppBundler in your own project you can add the following to your `pom.xml` file:

```xml
<dependency>
    <groupId>com.evolvedbinary.appbundler</groupId>
    <artifactId>appbundler</artifactId>
    <version>1.4.0</version>
</dependency>
```

The native part of the AppBundler artifact is built as a Universal binary that should run on both macOS for x86_64 and arm64 processors.
If you only need a platform specific binary, you may add a classifier to the dependency coordinates above of either: `<classifier>macos-x86_64-only</classifier>` or `<classifier>macos-arm64-only</classifier>`.

## Compiling

To build you will need a macOS machine with Git installed. You can then run:

```bash
$ git clone https://github.com/evolvedbinary/appbundler-maven-build.git
$ cd appbundler-maven-build
$ ./mvnw clean package
```

NOTE: If you are on a Windows platform you should replace `./mvnw` with `mvn.cmd`.
