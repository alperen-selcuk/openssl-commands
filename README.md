# openssl-commands

PFX formattaki bir sertifikadan crt ve key üretmek için

openssl pkcs12 -in wildcard.pfx -nocerts -out key.pem -nodes
openssl pkcs12 -in wildcard.pfx -clcerts -nokeys -out cert.pem
