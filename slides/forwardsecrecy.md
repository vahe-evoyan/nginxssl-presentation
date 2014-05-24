# Forward secrecy

## A+

Requires use of ephemeral Diffie-Hellman key exchange (ECDHE) to establish session keys.

```
ssl_ciphers "EECDH+ECDSA+AESGCM:EECDH+aRSA+AESGCM:EECDH+ECDSA+SHA384:EECDH+ECDSA+SHA256:EECDH+aRSA+SHA384:EECDH+aRSA+SHA256:EECDH:EDH+aRSA:!EDH-RSA-DES-CBC-SHA:!EXP-EDH-RSA-DES-CBC-SHA:!EECDH+aRSA+RC4:!RC4:!aNULL:!eNULL:!LOW:!3DES:!MD5:!EXP:!PSK:!SRP:!DSS"
```