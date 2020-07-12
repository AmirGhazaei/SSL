1. trust cert on server
  1.1 certutil -addstore -f "ROOT" new-root-certificate.crt

1. Convert pem to pfx
  1.1 openssl pkcs12 -inkey bob_key.pem -in bob_cert.cert -export -out bob_pfx.pfx
