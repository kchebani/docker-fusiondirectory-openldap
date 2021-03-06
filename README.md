docker-fusiondirectory-openldap
===============================

[![Travis Build Status](https://travis-ci.org/hrektts/docker-fusiondirectory-openldap.svg?branch=master)](https://travis-ci.org/hrektts/docker-fusiondirectory-openldap)
[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)

Dockerfile to build a [OpenLDAP](http://www.openldap.org/) container image that
includes the [FusionDirectory](https://www.fusiondirectory.org/) schemas.

Quick Start
-----------

You can launch the image using the docker command:

``` shell
docker run --name ldap -p 389:389 \
  -e LDAP_ORGANISATION="Example Organization" \
  -e LDAP_DOMAIN="example.org" \
  -e LDAP_ADMIN_PASSWORD="password" \
  -e FD_ADMIN_PASSWORD="fdadminpwd" \
  -d hrektts/fusiondirectory-openldap:latest
```

References
----------

[osixia/docker-openldap](https://github.com/osixia/docker-openldap)
