# Alpine PHP 

Repository of https://hub.docker.com/repository/docker/randef/alpine-php

[![Build Status](https://travis-ci.org/randef/alpine-php.svg?branch=master)](https://travis-ci.org/randef/alpine-php) ![Docker Pulls](https://img.shields.io/docker/pulls/randef/alpine-php.svg?style=flat-square)

Minimal PHP Docker images based on Alpine. Contains **tags** for development environments and adapted for various frameworks like [Symfony](http://symfony.com/) and [Wordpress](https://github.com/WordPress/WordPress).

## Documentation

[Read about Documentation and see some examples here](https://github.com/randef/alpine-php/tree/master/doc/README.md)

## Images

- [7.4](https://github.com/randef/alpine-php/blob/master/7.4/Dockerfile)
- [7.3](https://github.com/randef/alpine-php/blob/master/7.3/Dockerfile)
- [7.2](https://github.com/randef/alpine-php/blob/master/7.2/Dockerfile)
- [7.1](https://github.com/randef/alpine-php/blob/master/7.1/Dockerfile)

## Usage:

```sh
docker run -d --name dev -p 9000:9000 -p 2323:22 -v $PWD:/app randef/alpine-php:7.3-dev
```

> SSH is only for IDE integration to use container as remote interpreter 

## Dev Dockerfiles

Dev images extend the standard ones and add some tools for development and CI like, composer, xdebug, etc...

| General purpose     |                                                         
|---------------------|
| [7.4-dev](https://github.com/randef/alpine-php/blob/master/7.4/Dockerfile)|
| [7.3-dev](https://github.com/randef/alpine-php/blob/master/7.3/Dockerfile)|
| [7.2-dev](https://github.com/randef/alpine-php/blob/master/7.2/Dockerfile)|
| [7.1-dev](https://github.com/randef/alpine-php/blob/master/7.1/Dockerfile)|

## Content table

|    Tag     | Parent     |        Content                                                                    |
|------------|------------|-----------------------------------------------------------------------------------|
| 7.4        |   alpine   | tini, php7.4-cli & fpm                                                            | 
| 7.4-dev    |    7.4     | + SSH server, xdebug, ant, composer                                               | 
| 7.3        |   alpine   | tini, php7.3-cli & fpm                                                            | 
| 7.3-dev    |    7.3     | + SSH server, xdebug, ant, composer                                               |
| 7.2        |   alpine   | tini, php7.2-cli & fpm                                                            |
| 7.2-dev    |    7.2     | + SSH server, xdebug, ant, composer                                               |
| 7.1        |   alpine   | tini, php7.1-cli & fpm                                                            | 
| 7.1-dev    |    7.1     | + SSH server, xdebug, ant, composer                                               |
