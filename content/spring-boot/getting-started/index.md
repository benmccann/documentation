---
date: 2018-11-07T00:11:02+01:00
title: Getting started
weight: 10
menu:
  main:
    identifier: boot-getting-started
    parent: Spring Boot
    url: /spring-boot/getting-started/
---

This project requires at least the following version:

* Java 8
* Spring Boot > 2.x.x (`spring-boot-starter-web`)

## Quick start

To add `graphql-spring-boot` to your project and get started quickly, do the following.

### Build with Gradle

Make sure `mavenCentral` is amongst your repositories:
```gradle
repositories {
    mavenCentral()
}
```

Add the respective starter dependencies you want to use:
```gradle
dependencies {
    compile 'com.graphql-java-kickstart:graphql-spring-boot-starter:7.0.1'
    compile 'com.graphql-java-kickstart:graphiql-spring-boot-starter:7.0.1'
    compile 'com.graphql-java-kickstart:voyager-spring-boot-starter:7.0.1'
    testCompile 'com.graphql-java-kickstart:graphql-spring-boot-starter-test:7.0.1'
}
```

### Build with Maven

Add the respective starter dependencies you want to use:
```xml
<dependency>
  <groupId>com.graphql-java-kickstart</groupId>
  <artifactId>graphql-spring-boot-starter</artifactId>
  <version>7.0.1</version>
</dependency>
<dependency>
  <groupId>com.graphql-java-kickstart</groupId>
  <artifactId>graphiql-spring-boot-starter</artifactId>
  <version>7.0.1</version>
</dependency>
<dependency>
  <groupId>com.graphql-java-kickstart</groupId>
  <artifactId>voyager-spring-boot-starter</artifactId>
  <version>7.0.1</version>
</dependency>
<dependency>
  <groupId>com.graphql-java-kickstart</groupId>
  <artifactId>graphql-spring-boot-starter-test</artifactId>
  <version>7.0.1</version>
  <scope>test</scope>
</dependency>
```

## Using the latest development build

Snapshot versions of the current `master` branch are availble on JFrog. Check the next snapshot version on
[Github](https://github.com/graphql-java-kickstart/graphql-java-tools/blob/master/gradle.properties)

### Build with Gradle

Add the Snapshot repository:
```gradle
repositories {
    mavenCentral()
    maven { url "http://oss.jfrog.org/artifactory/oss-snapshot-local" }
}
```

### Build with Maven

Add the Snapshot repository:
```xml
<repositories>
  <repository>
    <id>oss-snapshot-local</id>
    <name>jfrog</name>
    <url>http://oss.jfrog.org/artifactory/oss-snapshot-local</url>
    <snapshots>
      <enabled>true</enabled>
      <updatePolicy>always</updatePolicy>
    </snapshots>
  </repository>
</repositories>
```
