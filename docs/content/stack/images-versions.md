---
title: "Stock Images versions"
weight: 6
---

## Understanding versions

Image tags follow the next pattern: 

    <image-repo>:<software-version>[-<image-stability-tag>][-<flavor>]

Take an example: `docksal/mysql:5.7-1.3`. 

`5.7` means software version, in this case MySQL 5.7. 

`1.3` means image stability tag. Stability tag is the image version. 
Same software version might have several image versions. 
Let's say we have added something to the MySQL 5.7 image (like a new default configuration), 
we would increase the stability tag to `1.4` in that case, but the software version `5.7` would remain the same,
resulting in `docksal/mysql:5.7-1.4` tag.

Note: `cli` is a special case, `cli` itself is seen as software here with `-php...` being just a flavor of it. 

## CLI

[![CLI on Github](https://img.shields.io/badge/Release%20notes-black.svg?logo=github&style=flat-square&classes=inline)](https://github.com/docksal/service-cli/releases)
[![CLI on Docker hub](https://img.shields.io/badge/View%20on%20Docker%20Hub-gray.svg?logo=docker&style=flat-square&classes=inline)](https://hub.docker.com/r/docksal/cli/tags)

| Image| Notes |
|------|------|
| `docksal/cli:2.9-php7.3` | *Default image* PHP 7.3, Nodejs v10.16.3, Ruby 2.6.4, Python 2.7.0, msmtp |
| `docksal/cli:2.9-php7.2` | PHP 7.2, Nodejs v10.16.3, Ruby 2.6.4, Python 2.7.0, msmtp |
| `docksal/cli:2.9-php7.1` | PHP 7.1, Nodejs v10.16.3, Ruby 2.6.4, Python 2.7.0, msmtp |
| `docksal/cli:2-php7.3`   | Latest 2.x image version of PHP 7.3 flavor, convenient when [extending images](/stack/extend-images)
| `docksal/cli:2-php7.2`   | Latest 2.x image version of PHP 7.2 flavor, convenient when [extending images](/stack/extend-images))
| `docksal/cli:2.5-php7.0` | *Deprecated*, PHP 7.0, mhsendmail |
| `docksal/cli:2.5-php5.6` | *Deprecated*, PHP 5.6, mhsendmail |

## Apache

[![Apache on Github](https://img.shields.io/badge/Release%20notes-black.svg?logo=github&style=flat-square&classes=inline)](https://github.com/docksal/service-apache/releases)
[![Apache on Docker hub](https://img.shields.io/badge/View%20on%20Docker%20Hub-gray.svg?logo=docker&style=flat-square&classes=inline)](https://hub.docker.com/r/docksal/apache/tags)

| Image| Notes |
|------|------|
| `docksal/apache:2.4-2.3` | *Default image*, Apache 2.4 |
| `docksal/apache:2.4`     | Apache 2.4 (latest) |

## Nginx 

[![Nginx on Github](https://img.shields.io/badge/Release%20notes-black.svg?logo=github&style=flat-square&classes=inline)](https://github.com/docksal/service-nginx/releases)
[![Nginx on Docker hub](https://img.shields.io/badge/View%20on%20Docker%20Hub-gray.svg?logo=docker&style=flat-square&classes=inline)](https://hub.docker.com/r/docksal/nginx/tags)

| Image| Notes |
|------|------|
| `docksal/nginx:1.15`     | Nginx 1.15 (latest 1.15 image version) |
| `docksal/nginx:1.15-1.0` | Nginx 1.15 (v. 1.0) |
| `docksal/nginx:1.14`     | Nginx 1.14 (latest 1.14 image version) |
| `docksal/nginx:1.14-1.0` | *Default image*, Nginx 1.14 (v. 1.0) |
| `docksal/nginx:1.13`     | Nginx 1.13 (latest 1.13 image version) |
| `docksal/nginx:1.13-1.0` | Nginx 1.13 (v. 1.0) |
| `docksal/nginx:1.12`     | Nginx 1.12 (latest 1.12 image version) |
| `docksal/nginx:1.12-1.0` | Nginx 1.12 (v. 1.0) |
| `docksal/nginx:1.11`     | Nginx 1.11 (latest 1.11 image version) |
| `docksal/nginx:1.11-1.0` | Nginx 1.11 (v. 1.0) |

## MySQL 

[![MySQL on Github](https://img.shields.io/badge/Release%20notes-black.svg?logo=github&style=flat-square&classes=inline)](https://github.com/docksal/service-mysql/releases)
[![MySQL on Docker hub](https://img.shields.io/badge/View%20on%20Docker%20Hub-gray.svg?logo=docker&style=flat-square&classes=inline)](https://hub.docker.com/r/docksal/mysql/tags)

| Image| Notes |
|------|------|
| `docksal/mysql:5.6`      | MySQL 5.6 (latest image version) |
| `docksal/mysql:5.6-1.4`  | *Default image*, MySQL 5.6 (v. 1.4) |
| `docksal/mysql:5.7`      | MySQL 5.7 (latest 5.7 image version) |
| `docksal/mysql:5.7-1.4`  | MySQL 5.7 (v. 1.4) |
| `docksal/mysql:8.0`      | MySQL 8.0 (latest 8.0 image version) |
| `docksal/mysql:8.0-1.4`  | MySQL 8.0 (v. 1.4) |

## MariaDB

[![MariaDB on Github](https://img.shields.io/badge/Release%20notes-black.svg?logo=github&style=flat-square&classes=inline)](https://github.com/docksal/service-mariadb/releases)
[![MariaDB on Docker hub](https://img.shields.io/badge/View%20on%20Docker%20Hub-gray.svg?logo=docker&style=flat-square&classes=inline)](https://hub.docker.com/r/docksal/mariadb/tags)

| Image| Notes |
|------|------|
| `docksal/mariadb:5.5`      | MariaDB 5.5 |
| `docksal/mariadb:10.0`     | MariaDB 10.0 |
| `docksal/mariadb:10.1`     | MariaDB 10.1 |
| `docksal/mariadb:10.2`     | MariaDB 10.2 |
| `docksal/mariadb:10.3`     | MariaDB 10.3 (latest) |

## Apache Solr

[![Solr on Github](https://img.shields.io/badge/Release%20notes-black.svg?logo=github&style=flat-square&classes=inline)](https://github.com/docksal/service-solr/releases)
[![Solr on Docker hub](https://img.shields.io/badge/View%20on%20Docker%20Hub-gray.svg?logo=docker&style=flat-square&classes=inline)](https://hub.docker.com/r/docksal/solr/tags)

| Image| Notes |
|------|------|
| `docksal/solr:5.5`      | Apache Solr 5.5 |
| `docksal/solr:6.6`      | Apache Solr 6.6 |
| `docksal/solr:7.5`      | Apache Solr 7.5 (latest) |


## Web 

**DEPRECATED:** Use `docksal/apache` or `docksal/nginx` instead

[![Web on Docker hub](https://img.shields.io/badge/View%20on%20Docker%20Hub-gray.svg?logo=docker&style=flat-square&classes=inline)](https://hub.docker.com/r/docksal/web/tags)

| Image| Notes |
|------|------|
| `docksal/web:apache2.4`     | Apache 2.4 |
| `docksal/web:apache2.2`     | Apache 2.2 |
