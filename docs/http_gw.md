# `neofs.http_gw` configuration

| Parameter | Description |
|-----------|-------------|
| `neofs_http__version` | Version of the binary to install. |
| `neofs_http__github_org` | GitHub user or organization to get the binary from. |
| `neofs_http__github_repo` | GitHub repository to get the binary from. |
| `neofs_http__github_asset_name` | GitHub release asset name. |
| `neofs_http__configure_only` | Skip binaries download. |
| `neofs_http__instance` | Optional prefix for multiple instances. |
| `neofs_http__user` | Name of the UNIX account used by the service. |
| `neofs_http__group` | Name of the UNIX group used by the service. |
| `neofs_http__conf_dir` | Absolute path to the directory with configuration files. |
| `neofs_http__bin_path` | Absolute path to the :command:`neofs-http-gw` binary installed on the host. |
| `neofs_http__wallet` | Path to the :file:`secret/` directory on the Ansible Controller to get the wallet from. |
| `neofs_http__wallet_path` | Absolute path to the wallet on the target host. |
| `neofs_http__wallet_address` | Account address. If omitted default one will be used. |
| `neofs_http__wallet_password` | Passphrase to decrypt the wallet. |
| `neofs_http__http_address` | Address to listen on. |
| `neofs_http__http_port` | Port to listen on. |
| `neofs_http__http_allow` | List of IP addresses or subnets that are allowed to connect to the service over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_http__http_group_allow` | List of IP addresses or subnets that are allowed to connect to the service over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_http__http_host_allow` | List of IP addresses or subnets that are allowed to connect to the service over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_http__prometheus_enabled` | When enabled, expose Prometheus monitoring metrics at a separate endpoint. |
| `neofs_http__prometheus_address` | Address for Prometheus monitoring metrics endpoint. |
| `neofs_http__prometheus_port` | Port for Prometheus monitoring metrics endpoint. |
| `neofs_http__prometheus_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_http__prometheus_group_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_http__prometheus_host_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_http__pprof_enabled` | When enabled, expose pprof at a separate endpoint. |
| `neofs_http__pprof_address` | Address for pprof endpoint. |
| `neofs_http__pprof_port` | Port for pprof endpoint. |
| `neofs_http__pprof_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_http__pprof_group_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_http__pprof_host_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_http__pool_error_threshold` | The number of errors on connection after which node is considered as unhealthy. |
| `neofs_http__raw_config` | The base for ``{{ neofs_http__conf_dir }}/config.yaml`` that will be extended with :envvar:`neofs_http__*config` |
| `neofs_http__default_config` | The default ``{{ neofs_http__conf_dir }}/config.yaml`` configuration provided by this role. |
| `neofs_http__config` | Additional ``{{ neofs_http__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory. |
| `neofs_http__group_config` | Additional ``{{ neofs_http__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory group. |
| `neofs_http__host_config` | Additional ``{{ neofs_http__conf_dir }}/config.yaml`` configuration that should be present on specific hosts in the Ansible inventory. |
| `neofs_http__combined_config` | The combined configuration variables that will be used to template the ``{{ neofs_http__conf_dir }}/config.yaml`` file |
| `neofs_http__debops_ferm_import` | Use debops.ferm role (via role import) |
| `neofs_http__ferm__dependent_rules` | Firewall configuration for the :ref:`debops.ferm` Ansible role. |
