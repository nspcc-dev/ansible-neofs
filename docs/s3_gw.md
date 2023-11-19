# `neofs.s3_gw` default variables

| Parameter | Description |
|-----------|-------------|
| `neofs_s3__version` | Version of the binary to install. |
| `neofs_s3__github_org` | GitHub user or organization to get the binary from. |
| `neofs_s3__github_repo` | GitHub repository to get the binary from. |
| `neofs_s3__gw_github_asset_name` | GitHub release asset name. |
| `neofs_s3__configure_only` | Skip binaries download. |
| `neofs_s3__user` | Name of the UNIX account used by the service. |
| `neofs_s3__group` | Name of the UNIX group used by the service. |
| `neofs_s3__conf_dir` | Absolute path to the directory with configuration files. |
| `neofs_s3__bin_path` | Absolute path to the :command:`neofs-s3-gw` binary installed on the host. |
| `neofs_s3__neofs_adm_config` | :command:`neofs-adm` config files on the Ansible Controller |
| `neofs_s3__alphabet_wallets` | Path to the alphabet wallets on the Ansible Controller |
| `neofs_s3__wallet` | Path to the :file:`secret/` directory on the Ansible Controller to get the wallet from. |
| `neofs_s3__wallet_path` | Absolute path to the wallet on the target host. |
| `neofs_s3__wallet_address` | Account address. If omitted default one will be used. |
| `neofs_s3__wallet_password` | Passphrase to decrypt the wallet. |
| `neofs_s3__s3_address` | Address to listen on. |
| `neofs_s3__s3_port` | Port to listen on. |
| `neofs_s3__prometheus_enabled` | When enabled, expose Prometheus monitoring metrics at a separate endpoint. |
| `neofs_s3__prometheus_address` | Address for Prometheus monitoring metrics endpoint. |
| `neofs_s3__prometheus_port` | Port for Prometheus monitoring metrics endpoint. |
| `neofs_s3__pprof_enabled` | When enabled, expose pprof at a separate endpoint. |
| `neofs_s3__pprof_address` | Address for pprof endpoint. |
| `neofs_s3__pprof_port` | Address for pprof endpoint. |
| `neofs_s3__pool_error_threshold` | The number of errors on connection after which node is considered as unhealthy. |
| `neofs_s3__raw_config` | The base for ``{{ neofs_s3__conf_dir }}/config.yaml`` that will be extended with :envvar:`neofs_s3__*config` |
| `neofs_s3__default_config` | The default ``{{ neofs_s3__conf_dir }}/config.yaml`` configuration provided by this role. |
| `neofs_s3__config` | Additional ``{{ neofs_s3__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory. |
| `neofs_s3__group_config` | Additional ``{{ neofs_s3__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory group. |
| `neofs_s3__host_config` | Additional ``{{ neofs_s3__conf_dir }}/config.yaml`` configuration that should be present on specific hosts in the Ansible inventory. |
| `neofs_s3__combined_config` | The combined configuration variables that will be used to template the ``{{ neofs_s3__conf_dir }}/config.yaml`` file |
