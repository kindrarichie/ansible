# Project0secrets

Certbot is a free, open source software tool for using Let’s Encrypt certificates on manually-administrated websites to enable HTTPS.
Secure communication over the Web relies on HTTPS, which requires the use of a digital certificate that lets browsers verify the identity of web servers. 
Web servers obtain their certificates from trusted third parties called certificate authorities (CAs). Certbot is an easy-to-use client that fetches a certificate from Let’s Encrypt—an open certificate authority.

- The file fullchain.pem is the signed certificate plus one or more certificates that make up the issuing CA chain. 
It is a concatenation of cert.pem (the “public key”) and chain.pem. 

- The file privkey.pem is the private key that was already used to sign the cert request.

- The options-ssl-apache.conf file is the Apache plugin for Certbot.  It includes SSL configuration for Apache from let's encrypt's configuration directory.