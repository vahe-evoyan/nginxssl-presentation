# Insecure ciphers and SSL/TLS versions

  - SSL v2.0 is insecure: flawed in a variety of ways
  - CBC ciphers in general are vulnerable to padding oracle attack and to BEAST
    up to TLS v1.0
  - RC4 used to mitigate the BEAST attack until latest demonstrations that
    it's broken
  - NULL ciphers

note:

- SSL 2.0
  - has a weak MAC construction that uses the MD5 hash function with a secret prefix, making it vulnerable to length extension attacks.
  - does not have any protection for the handshake, meaning a man-in-the-middle downgrade attack can go undetected
  - uses the TCP connection close to indicate the end of data
  - assumes a single service and a fixed domain certificate
- CBC
  - available also timing attacks "lucky 13", for the timing attack workaround 
- NULL ciphers
  - It would today be regarded as a simple form of steganography
- TLS 1.1, 1.2 are not vulnerable to BEAST

