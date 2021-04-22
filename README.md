# Ansible Role: Graylog



## Requirements

None.

## Role Variables



## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - ansible-graylog

## Example Inventory

- Standalone
```ini
[graylog]
graylog ansible_user=ubuntu ansible_host=x.x.x.x ansible_port=22
```
- Graylog Cluster
```ini
graylog-1 ansible_user=ubuntu ansible_host=x.x.x.x ansible_port=22
graylog-2 ansible_user=ubuntu ansible_host=x.x.x.x ansible_port=22
graylog-3 ansible_user=ubuntu ansible_host=x.x.x.x ansible_port=22

[graylog_master]
graylog-1

[graylog_worker]
graylog-2
graylog-3
```
## License

MIT

## Author Information

Opsta (Thailand) Co.,Ltd.
