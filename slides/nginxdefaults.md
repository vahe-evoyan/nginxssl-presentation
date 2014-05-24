# Nginx Defaults

## A-

The server does not support *Forward Secrecy* with the reference browsers.

```
ssl_session_cache none;
ssl_session_timeout 10m;

ssl_prefer_server_ciphers off;
ssl_protocols SSLv3 TLSv1 TLSv1.1 TLSv1.2;
ssl_ciphers HIGH:!aNULL:!MD5;
```