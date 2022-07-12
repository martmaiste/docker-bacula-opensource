# Bacula on Docker

## Introduction

Simplified docker version of Bacula (Open Source) 9.0.6 server including
Directory and Storage Daemon only. Images are based on CentOS Stream 8 and the
work is inspired by [RedCoolBeans](https://github.com/RedCoolBeans/docker-bacula-opensource)

The main goal for this project is to upgrade Bacula Directory and Storage
Daemon version on the CentOS 7 server to have Bacula 9 version with keeping the original configuration. 

## Installation and usage

Configuration files are expected to be in /etc/bacula. This image will not
create default database nor does it include default configuration files.
Tested with docker-ce 20.10.17 and docker-compose 1.18

Local build:
```
git clone https://github.com/martmaiste/docker-bacula-opensource.git
cd docker-bacula-opensource
docker-compose build
docker-compose up -d
docker-compose logs --follow
```

## Copyright and license

MIT, please see the LICENSE file.
