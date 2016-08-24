## Service security

* **OGC**
    - `<service>.<operation|*>=<roleA>[,<roleB>,<roleC>,etc]`
        + The *identifier* of an OGC service like **WMS**, **WFS**, **WCS**
        + Any *operation* for the specified service while wildcard is `*`
    - Examples of securing *WFS*:
        ```bash
        wfs.*=EMPLOYEE,MANAGER #restrict the whole WFS service
        ```
        ```bash
        wfs.GetFeature=EMPLOYEE,MANAGER #restrict WFS read-only operation
        wfs.Transaction=MANAGER #restrict WFS write operation
        ```
    >Limitation: **Service** and **Layer Security** cannot be combined. This doesn't allow to secure a specified OWS service just for a required layer. More with [GeoFence](http://docs.geoserver.org/stable/en/user/community/geofence-server/index.html)
