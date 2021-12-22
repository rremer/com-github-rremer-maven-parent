# com-github-rremer-maven-parent

[![Build Status](https://img.shields.io/travis/rremer/com-github-rremer-maven-parent)](https://travis-ci.org/rremer/com-github-rremer-maven-parent)
[![Site](https://img.shields.io/badge/site-1.0.3-green.svg)](https://rremer.github.io/com-github-rremer-maven-parent/1.0.3/index.html)
[![Maven Central](https://img.shields.io/badge/version-1.0.3-green.svg)](https://search.maven.org/artifact/com.github.rremer/maven-parent/1.0.3/pom)
![License](https://img.shields.io/github/license/rremer/com-github-rremer-maven-parent)
[![Keybase PGP](https://img.shields.io/keybase/pgp/rremer)](https://keybase.io/rremer/pgp_keys.asc)


Maven Parent POM for com.github.rremer projects.

## Usage

In your maven project ```pom.xml```, add:

```xml
<parent>
    <groupId>com.github.rremer</groupId>
    <artifactId>maven-parent</artifactId>
    <version>1.0.3</version>
</parent>
```

## Building

```sh
mvn clean install
```

## Releasing

```sh
mvn versions:set -DnewVersion=1.0.3
mvn clean deploy -Dparameter.gpg.skip=false
mvn site site-deploy
```

[per their instructions]:https://central.sonatype.org/pages/apache-maven.html
