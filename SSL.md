1. Trust cert on server
    1. Run Windows Power Shell or CMD as administrator
    1. certutil -addstore -f "ROOT" new-root-certificate.crt

1. Convert pem to pfx
    1. Install OpenSSL
    1. openssl pkcs12 -inkey bob_key.pem -in bob_cert.cert -export -out bob_pfx.pfx
