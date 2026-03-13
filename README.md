-- this readme is a draft --

# InfluxDB

Ansible role for installing and configuring InfluxDB.

## Requirements

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

## Role Variables

- `influxdb_upgrade`: Description. Default: `false`
- `influxdb_service_name`: Description. Default: `influxdb`
- `influxdb_backup_configs`: Description. Default: `false`
- `influxdb_conf_dir`: Description. Default: `/etc/influxdb`
- `influxdb_var_dir`: Description. Default: `/var/lib/influxdb`
- `influxdb_http_bind_address`: Description. Default: `:8086`
- `influxdb_auth_enabled`: Description. Default: `false`
- `influxdb_https_enabled`: Description. Default: `false`
- `influxdb_user`: Description.
- `influxdb_users`: Description.
- `influxdb_ssl_certs`: Description.
- `influxdb_ssl_certificate`: Description. Required if `influxdb_ssl_certs` is defined.
- `influxdb_ssl_certificate_key`: Description. Required if `influxdb_ssl_certs` is defined.

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: jdavcs.influxdb

## License

[MIT](LICENSE)
