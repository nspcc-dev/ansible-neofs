# `neofs.rest_gw` default variables

| Parameter | Description |
|-----------|-------------|
| `neofs_rest__version` | Version of the binary to install. |
| `neofs_rest__github_org` | GitHub user or organization to get the binary from. |
| `neofs_rest__github_repo` | GitHub repository to get the binary from. |
| `neofs_rest__github_asset_name` | GitHub release asset name. |
| `neofs_rest__binaries_download` | Skip binaries download. |
| `neofs_rest__user` | Name of the UNIX account used by the service. |
| `neofs_rest__group` | Name of the UNIX group used by the service. |
| `neofs_rest__conf_dir` | Absolute path to the directory with configuration files. |
| `neofs_rest__bin_path` | Absolute path to the :command:`neofs-rest-gw` binary installed on the host. |
| `neofs_rest__wallet` | Path to the :file:`secret/` directory on the Ansible Controller to get the wallet from. |
| `neofs_rest__wallet_path` | Absolute path to the wallet on the target host. |
| `neofs_rest__wallet_address` | Account address. If omitted default one will be used. |
| `neofs_rest__wallet_password` | Passphrase to decrypt the wallet. |
| `neofs_rest__external_address` | The IP and port to be shown in the API documentation. Defaults to: `'{{ neofs_rest__rest_address }}:{{ neofs_rest__rest_port }'` |
| `neofs_rest__rest_address` | Address to listen on. |
| `neofs_rest__rest_port` | Port to listen on. |
| `neofs_rest__rest_allow` | List of IP addresses or subnets that are allowed to connect to the service over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_rest__rest_group_allow` | List of IP addresses or subnets that are allowed to connect to the service over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_rest__rest_host_allow` | List of IP addresses or subnets that are allowed to connect to the service over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_rest__prometheus_enabled` | When enabled, expose Prometheus monitoring metrics at a separate endpoint. |
| `neofs_rest__prometheus_address` | Address for Prometheus monitoring metrics endpoint. |
| `neofs_rest__prometheus_port` | Address for Prometheus monitoring metrics endpoint. |
| `neofs_rest__prometheus_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_rest__prometheus_group_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_rest__prometheus_host_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_rest__pprof_enabled` | When enabled, expose pprof at a separate endpoint. |
| `neofs_rest__pprof_address` | Address for pprof endpoint. |
| `neofs_rest__pprof_port` | Port for pprof endpoint. |
| `neofs_rest__pprof_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_rest__pprof_group_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_rest__pprof_host_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_rest__pool_error_threshold` | The number of errors on connection after which node is considered as unhealthy. |
| `neofs_rest__node_dial_timeout` | Timeout to dial node. |
| `neofs_rest__healthcheck_timeout` | Timeout to check node health during rebalance. |
| `neofs_rest__rebalance_timer` | Interval to check nodes' health. |
| `neofs_rest__scheme` | The listeners to enable, this can be repeated and defaults to the schemes in the swagger spec. |
| `neofs_rest__cleanup_timeout` | Grace period for which to wait before killing idle connections. |
| `neofs_rest__graceful_timeout` | Grace period for which to wait before shutting down the server. |
| `neofs_rest__max_header_size` | Controls the maximum number of bytes the server will read parsing the request header's keys and values, including the request line. It does not limit the size of the request body. |
| `neofs_rest__listen_limit` | Limit the number of outstanding requests. |
| `neofs_rest__keep_alive` | Sets the TCP keep-alive timeouts on accepted connections. It prunes dead TCP connections ( e.g. closing laptop mid-download). |
| `neofs_rest__read_timeout` | Maximum duration before timing out read of the request. |
| `neofs_rest__write_timeout` | Maximum duration before timing out write of the response. |
| `neofs_rest__raw_config` | The base for ``{{ neofs_rest__conf_dir }}/config.yaml`` that will be extended with :envvar:`neofs_rest__*config` |
| `neofs_rest__default_config` | The default ``{{ neofs_rest__conf_dir }}/config.yaml`` configuration provided by this role. |
| `neofs_rest__config` | Additional ``{{ neofs_rest__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory. |
| `neofs_rest__group_config` | Additional ``{{ neofs_rest__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory group. |
| `neofs_rest__host_config` | Additional ``{{ neofs_rest__conf_dir }}/config.yaml`` configuration that should be present on specific hosts in the Ansible inventory. |
| `neofs_rest__combined_config` | The combined configuration variables that will be used to template the ``{{ neofs_rest__conf_dir }}/config.yaml`` file |
| `neofs_rest__debops_ferm_import` | Use debops.ferm role (via role import) |
| `neofs_rest__ferm__dependent_rules` | Firewall configuration for the :ref:`debops.ferm` Ansible role. |
