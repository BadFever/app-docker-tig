# docker-app-tig

## Usage

### Generate InfluxDB admin token

### Execute ansible role

```YAML
---
- hosts: all
  gather_facts: true
  become: true

  roles:
    - role: app-docker-tig
      vars:
        application_path: "/srv/app-docker-tig"
        influxdb_init_org: "organization01"
        influxdb_init_admin_token: "Some token"
        influxdb_init_password: "admin"
        

```
