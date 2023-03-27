# Airline Ticket Reservation System (ATRS)

![GitHub](https://img.shields.io/github/license/terasolunaorg/atrs)

Airline Ticket Reservation System (ATRS) is a sample application for developers to learn how to make applications with TERASOLUNA Server Framework for Java (5.x).

> **Note**
> [TERASOLUNA](https://terasolunaorg.github.io/) is a customized framework based on [Macchinetta](https://macchinetta.github.io/) by NTT DATA.
> TERASOLUNA shares [ATRS published on Macchinetta](https://github.com/Macchinetta/atrs) as a sample application.
> Therefore, we did not change the license headers and package names from ATRS of Macchinetta in this ATRS of TERASOLUNA.

## Version mapping

The version mapping between TERASOLUNA and Macchinetta in ATRS is [here](https://github.com/terasolunaorg/atrs/wiki/ATRS%E3%81%AE%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6).

## How to run the application

### Install PostgreSQL

You need to create a database of PostgreSQL on a local machine. (PostgreSQL can be downloaded via [here site](http://www.postgresql.org/download/).)

| Property      | Value    |
|:------------- |:-------- |
| database name | atrs     |
| user name     | postgres |
| password      | postgres |

### Insert test data

Execute the following command to initialize DB.  

```console
$ mvn sql:execute -f atrs-initdb/pom.xml
```

## For JDK 8

### Build

```console
$ mvn clean install
```

### Run application

```console
$ mvn cargo:run -pl atrs-web
```

### Web access

Access the following URL.

http://localhost:8080/atrs/

## For JDK 11 , JDK 17

### Build

```console
$ mvn clean install -P default
```

### Run application

```console
$ mvn cargo:run -P default -pl atrs-web
```

### Web access

Access the following URL.

http://localhost:8080/atrs/
