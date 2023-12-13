# `neofs.ir` default variables

| Parameter | Description |
|-----------|-------------|
| `neofs_ir__version` | Version of the binary to install. |
| `neofs_ir__github_org` | GitHub user or organization to get the binary from. |
| `neofs_ir__github_repo` | GitHub repository to get the binary from. |
| `neofs_ir__bin` | :command:`neofs-ir` binary name |
| `neofs_ir__cli_bin` | :command:`neofs-cli` binary name |
| `neofs_ir__arch` | Architecture to download binaries for. |
| `neofs_ir__configure_only` | Skip binaries download. |
| `neofs_ir__use_docker` | Run in service in docker |
| `neofs_ir__docker_image: 'nspccdev/neofs-ir` | Docker image to get. |
| `neofs_ir__instance` | Optional prefix for multiple instances. |
| `neofs_ir__user` | Name of the UNIX account used by the service. |
| `neofs_ir__group` | Name of the UNIX group used by the service. |
| `neofs_ir__conf_dir` | Absolute path to the directory with configuration files. |
| `neofs_ir__config_path` | Absolute path to the configuration file. |
| `neofs_ir__bin_path` | Absolute path to the :command:`neofs-ir` binary installed on the host. |
| `neofs_ir__cli_bin_path` | Absolute path to the :command:`neofs-cli` binary installed on the host. |
| `neofs_ir__control_api_config_path` | Absolute path to the control API config path. |
| `neofs_ir__data_dir` | Directory for databases and processing results |
| `neofs_ir__wallet` | Path to the :file:`secret/` directory on the Ansible Controller to get the wallet from. |
| `neofs_ir__wallet_path` | Absolute path to the wallet on the target host. |
| `neofs_ir__wallet_address` | Account address. If omitted default one will be used. |
| `neofs_ir__wallet_password` | Passphrase to decrypt the wallet. |
| `neofs_ir__control_enabled` | When enabled, expose control at a separate endpoint. |
| `neofs_ir__control_address` | Address for control endpoint. |
| `neofs_ir__control_port` | Port for control endpoint. |
| `neofs_ir__control_allow` | List of IP addresses or subnets that are allowed to connect to the control endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__control_group_allow` | List of IP addresses or subnets that are allowed to connect to the control endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__control_host_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__prometheus_enabled` | When enabled, expose Prometheus monitoring metrics at a separate endpoint. |
| `neofs_ir__prometheus_address` | Address for Prometheus monitoring metrics endpoint. |
| `neofs_ir__prometheus_port` | Port for Prometheus monitoring metrics endpoint. |
| `neofs_ir__prometheus_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__prometheus_group_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__prometheus_host_allow` | List of IP addresses or subnets that are allowed to connect to the Prometheus endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__pprof_enabled` | When enabled, expose pprof at a separate endpoint. |
| `neofs_ir__pprof_address` | Address for pprof endpoint. |
| `neofs_ir__pprof_port` | Port for pprof endpoint. |
| `neofs_ir__pprof_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__pprof_group_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__pprof_host_allow` | List of IP addresses or subnets that are allowed to connect to the pprof endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__external_sidechain` | Enable or disable support internal sidechain. |
| `neofs_ir__blockchain_database_path` | Absolute path to the database file. |
| `neofs_ir__blockchain_notary_disabled` | Enable or disable notary mode for sidechain. |
| `neofs_ir__blockchain_time_per_block` | Minimal (and targeted for) time interval between blocks. Must be an integer number of milliseconds. |
| `neofs_ir__blockchain_magic` | Magic number which uniquely identifies Neo network. |
| `neofs_ir__blockchain_seed_nodes` | Optional list of existing nodes to communicate with over Neo P2P protocol. By default, node runs as standalone |
| `neofs_ir__blockchain_rpc_address: ':` | Address for RPC endpoint. |
| `neofs_ir__blockchain_rpc_port` | Port for RPC endpoint. |
| `neofs_ir__blockchain_rpc_allow` | List of IP addresses or subnets that are allowed to connect to the RPC endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__blockchain_rpc_group_allow` | List of IP addresses or subnets that are allowed to connect to the RPC endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__blockchain_rpc_host_allow` | List of IP addresses or subnets that are allowed to connect to the RPC endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__blockchain_rpc_addresses: [ '{{ neofs_ir__blockchain_rpc_address | ansible.utils.ipwrap }}` | List of network addresses to listen Neo RPC on. |
| `neofs_ir__blockchain_tls_rpc_enabled` | Enable or disable TLS RPC endpoint. |
| `neofs_ir__blockchain_tls_rpc_address: ':` | Address for TLS RPC endpoint. |
| `neofs_ir__blockchain_tls_rpc_port` | Port for TLS RPC endpoint. |
| `neofs_ir__blockchain_tls_rpc_allow` | List of IP addresses or subnets that are allowed to connect to the TLS RPC endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__blockchain_tls_rpc_group_allow` | List of IP addresses or subnets that are allowed to connect to the TLS RPC endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__blockchain_tls_rpc_host_allow` | List of IP addresses or subnets that are allowed to connect to the TLS RPC endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__blockchain_tls_rpc_addresses: [ '{{ neofs_ir__blockchain_tls_rpc_address | ansible.utils.ipwrap }}` | List of network addresses to listen Neo TLS RPC on. |
| `neofs_ir__blockchain_tls_rpc_cert` | Absolute path to the TLS certificate for RPC endpoint. |
| `neofs_ir__blockchain_tls_rpc_key` | Absolute path to the TLS key for RPC endpoint on the target host. |
| `neofs_ir__blockchain_tls_rpc_local_cert` | Path to the :file:`secret/` directory on the Ansible Controller to get TLS certificate for RPC endpoint from. |
| `neofs_ir__blockchain_tls_rpc_local_key` | Path to the :file:`secret/` directory on the Ansible Controller to get TLS key for RPC endpoint from. |
| `neofs_ir__blockchain_p2p_address: ':` | Address for P2P endpoint. |
| `neofs_ir__blockchain_p2p_port` | Port for P2P endpoint. |
| `neofs_ir__blockchain_p2p_allow` | List of IP addresses or subnets that are allowed to connect to the P2P endpoint over the network, configured on all hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__blockchain_p2p_group_allow` | List of IP addresses or subnets that are allowed to connect to the P2P endpoint over the network, configured on hosts in a specific Ansible inventory group. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__blockchain_p2p_host_allow` | List of IP addresses or subnets that are allowed to connect to the P2P endpoint over the network, configured on specific hosts in the Ansible inventory. If no entries are specified, access through the firewall is disabled. |
| `neofs_ir__blockchain_p2p_addresses: [ '{{ neofs_ir__blockchain_p2p_address | ansible.utils.ipwrap }}` | List of network addresses to listen Neo P2P on. |
| `neofs_ir__validators` | List of hex-encoded 33-byte public keys of sidechain validators to vote for at application startup. |
| `neofs_ir__consensus_committee` | List of hex-encoded 33-byte public keys. |
| `neofs_ir__mainnet_endpoints` | List of websocket RPC endpoints in mainchain. |
| `neofs_ir__morph_endpoints: [ 'ws://localhost` | List of websocket RPC endpoints in sidechain. |
| `neofs_ir__sidechain_config` | Local consensus config part. |
| `neofs_ir__raw_config` | The base for ``{{ neofs_ir__conf_dir }}/config.yaml`` that will be extended with :envvar:`neofs_ir__*config` |
| `neofs_ir__default_config` | The default ``{{ neofs_ir__conf_dir }}/config.yaml`` configuration provided by this role. |
| `neofs_ir__config` | Additional ``{{ neofs_ir__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory. |
| `neofs_ir__group_config` | Additional ``{{ neofs_ir__conf_dir }}/config.yaml`` configuration that should be present on all hosts in the Ansible inventory group. |
| `neofs_ir__host_config` | Additional ``{{ neofs_ir__conf_dir }}/config.yaml`` configuration that should be present on specific hosts in the Ansible inventory. |
| `neofs_ir__combined_config` | The combined configuration variables that will be used to template the ``{{ neofs_ir__conf_dir }}/config.yaml`` file |
| `neofs_ir__debops_ferm_import` | Use debops.ferm role (via role import) |
| `neofs_ir__ferm__dependent_rules` | Firewall configuration for the :ref:`debops.ferm` Ansible role. |
