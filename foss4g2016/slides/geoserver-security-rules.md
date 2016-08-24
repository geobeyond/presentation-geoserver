## AuthZ rules

### Data management

* Provides security rules at **[*data level*](http://docs.geoserver.org/stable/en/user/security/webadmin/data.html)** (no restrictions by default)
* You can combine **Workspace**, **Layer**, **Permission** (Setting *READ* or *WRITE* access mode) and **Roles** for each rule
* You can configure how secured layers are accessed by unauthorized users in the **Catalog Mode** : *HIDE*, *MIXED*, *CHALLENGE*

### Service management

* Provides security rules at **[*service level*](http://docs.geoserver.org/stable/en/user/security/webadmin/services.html)** (no restrictions by default)
* You can combine type of **OWS service** (basically *WMS*, *WFS*, *WCS*), **Operation** (meaning *GetMap*, etc) and **Roles** for each rule
* You can also manage to securing REST services by combining **Request URIs** with pattern matching expressions, **HTTP Method** and **Roles** for each rule
