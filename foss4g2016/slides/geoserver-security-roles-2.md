## Calculate Roles

![Role Calculation](css/img/usergrouprole1.png "Role Calculation")
* How to get roles
    * Using the [user/group service](http://docs.geoserver.org/stable/en/user/security/usergrouprole/usergroupservices.html#security-rolesystem-usergroupservices) for retrieving from the active *role service*
    * Directly through the configured *role service* (Limitations: no group memberships - no custom roles)
    * Using an *HTTP header attribute* :
        * Roles are received from a *Proxy AuthN* (Name of the header can be configured)
        ```conf
        my_roles: manager;approver;employee
        ```


