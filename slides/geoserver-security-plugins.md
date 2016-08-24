## Security Plugins

- [**GeoFence**](http://docs.geoserver.org/stable/en/user/community/geofence-server/index.html)
    + Advanced security AuthZ which allows rules that overcome the limitation on **Service** and **Layer Security** combination
    + Distributed as standalone or internal server with some limitations, it works with a rule database and can be configured through web interface or a REST API
    + Can be configured against a [LDAP Server](https://github.com/geoserver/geofence/wiki/GeoFence-configuration)
- [**CAS**](https://www.apereo.org/projects/cas)
    + Single Sign-On mechanism for AuthN
    + Supports LDAP Server V3 and database for user management
    + Supports for multiple protocols (*SAML*, *OAuth*, *OpenID*), essentially federation
- You can find a lot of useful documentation on how to configure and set these two plugins for implementing you security model in **GeoServer**
