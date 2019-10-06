# com-github-rremer-maven-parent

[![Build Status](https://travis-ci.org/rremer/com-github-rremer-maven-parent.svg?branch=master)](https://travis-ci.org/rremer/com-github-rremer-maven-parent)

Maven Parent POM for com.github.rremer projects.

## Usage

In your maven project ```pom.xml```, add:

```xml
<parent>
    <groupId>com.github.rremer</groupId>
    <artifactId>maven-parent</artifactId>
    <version>1.0.0</version>
</parent>
```

## Building

```sh
mvn clean install
```

## Releasing

Ensure your gpg key is installed and ```settings.xml``` is updated with id oss.sonatype.org [per their instructions].

```sh
mvn versions:set -DnewVersion=1.0.1
mvn clean deploy -Dparameter.gpg.skip=false
```

[per their instructions]:https://central.sonatype.org/pages/apache-maven.html
