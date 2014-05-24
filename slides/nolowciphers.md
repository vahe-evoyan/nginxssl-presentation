# Low encryption cipher suites

Disable all *low* encryption cipher suites, currently those using 64 or 56 bit encryption algorithms but excluding export cipher suites.

```
ssl_protocols SSLv3 TLSv1 TLSv1.1 TLSv1.2;
ssl_ciphers "ALL:!aNULL:!eNULL:!EXP:!LOW";
```

### Result: A-