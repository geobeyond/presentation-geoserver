## Serve Roles

* Type of persistence:
    * **XML file** : default [XML role service](http://docs.geoserver.org/stable/en/user/security/usergrouprole/roleservices.html#xml-role-service) within the file `roles.xml` at the relative path `security/role/<role service name>/roles.xml` in the **GEOSERVER_DATA_DIR**
    * **JDBC database** : [JDBC role service](http://docs.geoserver.org/stable/en/user/security/usergrouprole/roleservices.html#jdbc-role-service) in multiple tables: *roles* (primary table with parents), *role_props*, *user_roles*, *group_roles*
    * **J2EE deployment descriptor** : [J2EE role service](http://docs.geoserver.org/stable/en/user/security/usergrouprole/roleservices.html#j2ee-role-service) is **read-only** from XML elements: `<security-role>` - `<security-constraint>` - `<security-role-ref>`
    * **LDAP directory server** : [LDAP role service](http://docs.geoserver.org/stable/en/user/security/usergrouprole/roleservices.html#ldap-role-service) is **read-only** from a directory tree: each entry (groups) under a **group search base** is mapped to a role
    ```xml
        <groupSearchBase>ou=groups</groupSearchBase>
        <groupSearchFilter>uniquemember=uid={0},ou=people,dc=example,dc=com</groupSearchFilter>
    ```

