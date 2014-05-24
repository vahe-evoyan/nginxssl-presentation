## The Handshake

1. Negotiation
  * Client Hello (SSL version number, cipher settings, 
    session-specific data, etc.)
  * Server Hello (SSL version number, cipher settings, 
    session-specific data, etc. and certificate)
2. Key exchange
  * Client sends the encrypted pre-master secret to the server
  * Server decrypts the pre-master secret using its private key
  * Both perform a series of steps to generate the master secret
3. Secure communication

note:
  - In point 1 also possible client certificate validation
  - ![handshake](http://awakenaware.org/wp-content/uploads/2014/04/BasicSSLConnection.jpg)