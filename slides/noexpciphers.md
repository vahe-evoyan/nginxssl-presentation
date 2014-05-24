# Export cipher suites

Disable all 40 and 56 bits algorithms for export.

```
ssl_protocols SSLv3 TLSv1 TLSv1.1 TLSv1.2;
ssl_ciphers "ALL:!aNULL:!eNULL:!EXP";
```

### Result: B