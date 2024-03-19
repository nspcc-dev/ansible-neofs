# NSPCC NeoFS ansible collection

Ansible roles for [NeoFS][neofs]:
 - [IR][neofs-node]
 - [Storage][neofs-node]
 - [REST Gateway][neofs-rest-gw]
 - [S3 Gateway][neofs-s3-gw]


[neofs]:         https://fs.neo.org
[neospcc]:       https://nspcc.io
[neofs-node]:    https://github.com/nspcc-dev/neofs-node
[neofs-s3-gw]:   https://github.com/nspcc-dev/neofs-s3-gw
[neofs-rest-gw]: https://github.com/nspcc-dev/neofs-rest-gw

### Usage and configuration

For available configuration settings check the role page:
 - [ir][ir]
 - [storage][storage]
 - [s3-gw][s3-gw]
 - [rest-gw][rest-gw]

For real usage example check [ansible-neofs-template][ansible-neofs-template].

[ir]:      docs/ir.md
[storage]: docs/storage.md
[s3-gw]:   docs/s3_gw.md
[rest-gw]: docs/rest_gw.md
[ansible-neofs-template]: https://github.com/nspcc-dev/ansible-neofs-template


### Compatibility Table

| NeoFS Node | collection |
|------------|------------|
|     0.37.0 |      0.0.1 |

### To migrate from old roles

just add `nspcc.neofs` to `collections` array or call roles with `nspcc.neofs.` prefix.
