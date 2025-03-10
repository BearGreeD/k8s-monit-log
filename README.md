OC: Debian 12
------------------------------------------------------------------
.
├── ansible.cfg
├── group_vars
│   └── all
│       └── vars.yml
├── hosts
├── host_vars
│   └── prometheus_local.yml
├── prometheus_install.yml
└── roles
    ├── base
    │   ├── defaults
    │   │   └── main.yml
    │   ├── files
    │   │   ├── bashrc
    │   │   └── vimrc
    │   └── tasks
    │       ├── base_config.yml
    │       ├── base_files.yml
    │       ├── install_packages.yml
    │       └── main.yml
    ├── elastic_kibana
    │   ├── defaults
    │   │   └── main.yml
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   └── main.yml
    │   └── templates
    │       ├── elastic
    │       └── kibana
    ├── firewall
    │   ├── defaults
    │   │   └── main.yml
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   ├── disable_firewalld.yml
    │   │   ├── install_iptables.yml
    │   │   ├── iptables_rules.yaml
    │   │   └── main.yml
    │   └── templates
    │       └── iptables.j2
    ├── fluentbit
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   └── main.yml
    │   └── templates
    │       └── fluent-bit.conf.j2
    ├── node_exporter
    │   ├── defaults
    │   │   └── main.yml
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   └── main.yml
    │   └── templates
    │       └── node_exporter.service.j2
    └── prometheus
        ├── defaults
        │   └── main.yml
        ├── handlers
        │   └── main.yml
        ├── tasks
        │   └── main.yml
        └── templates
            ├── prometheus.service.j2
            └── prometheus.yml.j2
