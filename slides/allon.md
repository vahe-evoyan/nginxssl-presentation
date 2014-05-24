# Worst configuration

## All SSL versions and ciphers are turned on

```
ssl_protocols SSLv2 SSLv3 TLSv1 TLSv1.1 TLSv1.2;
ssl_ciphers "ALL";
```

### Result: F
  - This server supports SSL 2, which is obsolete and insecure.
  - This server supports anonymous (insecure) suites.

note:
  - remember, we don't have a Heartbleed here, though it would give the same
    result in the SSLLabs.