# GeoServer Security Model

- Based on [Spring Security](http://static.springsource.org/spring-security/site/)
- *Access Management*:
    - Authentication (**AuthN**)
        - [filters](http://docs.geoserver.org/stable/en/user/security/webadmin/auth.html#authentication-filters), [providers](http://docs.geoserver.org/stable/en/user/security/webadmin/auth.html#authentication-providers), [chain](http://docs.geoserver.org/stable/en/user/security/webadmin/auth.html#authentication-chain)
    - Authorization (**AuthZ**)
        - [Groups](http://docs.geoserver.org/stable/en/user/security/webadmin/ugr.html#add-group), [Roles](http://docs.geoserver.org/stable/en/user/security/webadmin/ugr.html#role-services), [Data](http://docs.geoserver.org/stable/en/user/security/webadmin/data.html), [Services](http://docs.geoserver.org/stable/en/user/security/webadmin/services.html)
- *Identity Management*:
    - Internal provider
    - External providers
