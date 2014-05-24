# Extra

### Session resumption

Session reuse improves SSL performance by submitting an appropriate blob to the server, a client is able to trigger an abbreviated handshake, improving latency and computation time.

```
ssl_session_cache shared:SSL:50m;
ssl_session_timeout 5m;
```

### Server ciphers

Server ciphers should be preferred over client ciphers.

```
ssl_prefer_server_ciphers on;
```

note:
 - When the server sends the “Server Hello” message, it can include a session identifier. The client should store it and present it in the “Client Hello” message of the next session. If the server finds the corresponding session in its cache and accepts to resume the session, it will send back the same session identifier and will continue with the abbreviated SSL handshake. Otherwise, it will issue a new session identifier and switch to a full handshake.