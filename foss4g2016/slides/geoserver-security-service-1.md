## Service security

* **REST**
    - `<uriPattern>;<method>[,<method>,etc]=<roleA>[,<roleB>,<roleC>,etc]`
        + An [ant pattern](http://docs.geoserver.org/stable/en/user/security/service.html#security-service-ant-patterns) that matches requests
        + The method of **HTTP** request (*GET*, *POST*, *PUT*, *POST*, *DELETE*, *HEAD*)
        + Name of the *Role* while wildcard is `*` and include anonymous users
    - Examples:
        ```bash
        /**;GET,POST,PUT,DELETE=ROLE_ADMINISTRATOR #Restrict any rest call to administrators
        ```

        ```bash
        /rest/**/states*;GET,POST=MANAGER #Restrict a specific resource (feature type)
        ```
