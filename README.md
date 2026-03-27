# InfluxDB

Ansible role for installing and configuring InfluxDB.

## Role Variables

| variable | default | required |
|:---|:---|:---:|
| influxdb_upgrade | `false` ||
| influxdb_backup_configs | `false` ||
| influxdb_conf_dir | `/etc/influxdb` ||
| influxdb_var_dir | `/var/lib/influxdb` ||
| influxdb_auth_enabled | `false` ||
| influxdb_https_enabled | `false` ||
| influxdb_http_protocol | `http://` or `https://` ||
| influxdb_http_host | `localhost` ||
| influxdb_http_bind_address | `:8086` ||
| influxdb_http_service_uri | protocol + host + bind_address ||
| influxdb_admin_user || yes|
| influxdb_admin_password || yes |
| influxdb_users |||
| influxdb_ssl_certs |||
| influxdb_ssl_certificate || yes, if `influxdb_ssl_certs` is defined |
| influxdb_ssl_certificate_key || yes, if `influxdb_ssl_certs` is defined |

## Example Playbook

```
- hosts: servers
  roles:
     - role: jdavcs.influxdb
```

## License

[MIT](LICENSE)
