# NSPCC NeoFS ansible collection

Ansible roles for [NeoFS][neofs]:
 - [IR][neofs-node]
 - [Storage][neofs-node]
 - [REST Gateway][neofs-rest-gw]
 - [S3 Gateway][neofs-s3-gw]
 - [HTTP Gateway][neofs-http-gw]


[neofs]:         https://fs.neo.org
[neospcc]:       https://nspcc.io
[neofs-node]:    https://github.com/nspcc-dev/neofs-node
[neofs-http-gw]: https://github.com/nspcc-dev/neofs-http-gw
[neofs-s3-gw]:   https://github.com/nspcc-dev/neofs-s3-gw
[neofs-rest-gw]: https://github.com/nspcc-dev/neofs-rest-gw

### Compatibility Table

| NeoFS Node | collection |
|------------|------------|
|     0.37.0 |      0.0.1 |

### To migrate from old roles

just add `nspcc.neofs` to `collections` array or call roles with `nspcc.neofs.` prefix.
