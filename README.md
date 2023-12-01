# openssl-commands

PFX formattaki bir sertifikadan crt ve key üretmek için

```
openssl pkcs12 -in wildcard.pfx -nocerts -out key.pem -nodes

openssl pkcs12 -in wildcard.pfx -clcerts -nokeys -out cert.pem
```

self-sign sertifika üretmek için

openssl req  -addext "subjectAltName = DNS:example.devopsdude.world" -newkey rsa:4096 -nodes -sha256 -keyout devopsdude.key -x509 -days 365 -out devopsdude.crt
