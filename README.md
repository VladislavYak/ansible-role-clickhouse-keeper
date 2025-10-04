Role Name
=========

Clickhouse role for deploying Clickhouse-keeper

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

```
keeper_port: 9181
keeper_raft_port: 9234

clickhouse_group: clickhouse
clickhouse_user: clickhouse
```

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
  - name: ClickHouse-Keeper
    hosts: keeper_cluster
    become: true

    roles:
      - role: ansible-role-clickhouse-keeper
```

License
-------

BSD

Author Information
------------------

Not tested with several CH-keeper servers yet.