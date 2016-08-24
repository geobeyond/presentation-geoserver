## Layer security

* `<workspace>.<layer>.<permission>=<roleA>[,<roleB>,<roleC>,etc]`
    - Name of **workspace** while wildcard is `*`
    - Name of a **layer** resource like *featuretype*, *coverage*, etc while wildcard, meaning all layers, is `*`
    - **permission** can be expressed with 3 types of access mode:
        - `r` - **Read mode** (read data from a *workspace*/*layer*)
        - `w` - **Write mode** (write data from a *workspace*/*layer*)
        - `a` - **Admin mode** (edit the configuration of a *workspace*/*layer*)
    - Names which contain dots can be expressed with **double backslashes** : `workspace.name\\.with.\\dots.permission=MANAGER`
```text
*.*.r=EMPLOYEE
*.*.w=MANAGER
topp.*.r=*
topp.states.r=CITIZEN
topp.states.w=EMPLOYEE
 ```

