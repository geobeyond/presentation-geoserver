# Filter vs Provider chain

![Filter chain](css/img/auth_chain2.png "Filter chain")

* **Provider** performs the authentication
* **Filter** select the authN scheme to apply for the current request. Basically, for instance, if an authentication is required or not
* **Filters** can be separated by *request type* with different *matching rules*: **HTTP method** - **ANT patterns** - **Regular expressions** for *query string* parameters
```
            /wfs|(?=.*request=getfeature)(?=.*format=application/json).*
```
