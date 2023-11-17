# `neofs.storage` default variables

| Parameter | Description |
|-----------|-------------|
| `neofs_storage__version` | Version of the binary to install. |
| `neofs_storage__github_org` | GitHub user or organization to get the binary from. |
| `neofs_storage__github_repo` | GitHub user or organization to get the binary from. |
| `neofs_storage__bin` | :command:`neofs-node` binary name |
| `neofs_storage__cli_bin` | :command:`neofs-cli` binary name |
| `neofs_storage__arch` | Architecture to download binaries for. |
| `neofs_storage__configure_only` | Skip binaries download. |
| `neofs_storage__use_docker` | Run service in Docker. |
| `neofs_storage__docker_image: 'nspccdev/neofs-ir` | Docker image to get. |
| `neofs_storage__instance` | Optional prefix for multiple instances. |
| `neofs_storage__user` | Name of the UNIX account used by the service. |
| `neofs_storage__group` | Name of the UNIX group used by the service. |
| `neofs_storage__conf_dir` | Absolute path to the directory with configuration files. |
| `neofs_storage__config_path` | Absolute path to the configuration file. |
| `neofs_storage__bin_path` | Absolute path to the :command:`neofs-node` binary installed on the host. |
| `neofs_storage__cli_bin_path` | Absolute path to the :command:`neofs-cli` binary installed on the host. |
| `neofs_storage__control_api_config_path` | Absolute path to the control API config path. |
| `neofs_storage__data_dir` | Absolute path for directory to store data. |
| `neofs_storage__meta_dir` | Absolute path for directory to store meta. |
| `neofs_storage__data_parts` | Data parts number. |
| `neofs_storage__meta_parts` | Meta parts number. |
| `neofs_storage__neofs_adm_config` | Path to the neofs_adm config file. |
| `neofs_storage__alphabet_wallets` | Path to the directory with alphabet wallet. |
| `neofs_storage__wallet` | Path to a file in :file:`secret/` directory to store password. |
| `neofs_storage__wallet_initial_gas` | Initial gas amount to generate new wallet with. |
| `neofs_storage__wallet_path` | Absolute path to the wallet on the target host. |
| `neofs_storage__wallet_address` | Account address. If omitted default one will be used. |
| `neofs_storage__wallet_password` | Passphrase to decrypt the wallet. |
| `neofs_storage__morph_endpoints` | Sidechain NEO RPC endpoints. |
| `neofs_storage__announce_addresses: [ '{{ neofs_storage__grpc_address | ansible.utils.ipwrap }}` | List of addresses to announce to the Network map. |
| `neofs_storage__grpc_address: ':` | Address for gRPC endpoint |
| `neofs_storage__grpc_port` | Port for gRPC endpoint |
| `neofs_storage__grpcs_port` | Port for gRPCs endpoint |
| `neofs_storage__grpc_allow` | List of IP addresses or subnets that are allowed to connect to the gRPC endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__grpc_group_allow` | List of IP addresses or subnets that are allowed to connect to the gRPC endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__grpc_host_allow` | List of IP addresses or subnets that are allowed to connect to the gRPC endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__tls_enabled` | Enable or disable gRPCs endpoint. |
| `neofs_storage__tls_cert` | Absolute path to the TLS certificate for gRPCs endpoint. |
| `neofs_storage__tls_key` | Absolute path to the TLS key for gRPCs endpoint. |
| `neofs_storage__tls_cert_file` | Absolute path to the TLS certificate for gRPCs endpoint. |
| `neofs_storage__tls_key_file` | Absolute path to the TLS key for gRPCs endpoint. |
| `neofs_storage__control_enabled` | When enabled, expose control at a separate endpoint. |
| `neofs_storage__control_address` | Address for control endpoint. |
| `neofs_storage__control_port` | Port for control endpoint. |
| `neofs_storage__control_allow` | List of IP addresses or subnets that are allowed to connect to the control endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__control_group_allow` | List of IP addresses or subnets that are allowed to connect to the control endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__control_host_allow` | List of IP addresses or subnets that are allowed to connect to the control endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__prometheus_enabled` | When enabled, expose Prometheus monitoring metrics at a separate endpoint. |
| `neofs_storage__prometheus_address` | Address for Prometheus monitoring metrics endpoint. |
| `neofs_storage__prometheus_port` | Port for Prometheus monitoring metrics endpoint. |
| `neofs_storage__prometheus_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__prometheus_group_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__prometheus_host_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__pprof_enabled` | When enabled, expose pprof at a separate endpoint. |
| `neofs_storage__pprof_address` | Address for pprof endpoint. |
| `neofs_storage__pprof_port` | Port for pprof endpoint. |
| `neofs_storage__pprof_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__pprof_group_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__pprof_host_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_storage__grpc_endpoints` | List of grpc enpoints. |
| `neofs_storage__grpc` | gRPC config part. |
| `neofs_storage__grpc_ferm_rules` | Firewall configuration for the :ref:`debops.ferm` Ansible role. |
| `neofs_storage__config` | Additional ``{{ neofs_storage__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory. |
| `neofs_storage__group_config` | Additional ``{{ neofs_storage__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory group. |
| `neofs_storage__host_config` | Additional ``{{ neofs_storage__conf_dir }}/config.yaml`` configuration that should be present on specific hosts in the Ansible inventory. |
| `neofs_storage__combined_config` | The combined configuration variables that will be used to template the ``{{ neofs_storage__conf_dir }}/config.yaml`` file |
| `neofs_storage__debops_ferm_import` | Use debops.ferm role (via role import) |
| `neofs_storage__ferm__dependent_rules` | Firewall configuration for the :ref:`debops.ferm` Ansible role. |
