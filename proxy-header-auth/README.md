# Proxy Header Authentication

![](img/proxy-header-auth.png)

This schema represents the concept and not the exact architcture in the code.
## Run

```
docker-compose up
```

## Usage

The following apps are available:

* http://app1.localhost
    * Authentication (auth_basic) required
    * Credentials: user/password OR user2/password2
* http://app2.localhost
    * Authentication (auth_basic) required
    * Credentials: user/password OR user2/password2;

Apps trust a HTTP header set by the proxy as an authenticated user. In this example, the header is set based on auth_basic.

## Screenshots

![](img/tandoor-header-auth.png)
![](img/firefly-header-auth.png)