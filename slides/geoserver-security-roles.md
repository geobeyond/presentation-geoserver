## Roles

* Entities with a *name* - *parents* - *set of key/value pairs* associated to certain **granted privileges** and **permitted resources**
* Can be assigned to users and groups of them
* Support **inheritance**
* Reserved *System Roles*:
    * **ROLE_ADMINISTRATOR** - allows all operations and access all resources
    * **ROLE_GROUP_ADMIN** - limited for administrating user groups
    * **ROLE_AUTHENTICATED** - specific to all authenticated users
    * **ROLE_ANONYMOUS** - specific to not authenticated users (when anonymous authn is enabled)
