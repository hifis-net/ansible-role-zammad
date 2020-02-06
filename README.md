# Ansible role: Zammad


An Ansible Role that installs Zammad on Linux.

## Requirements

This role has no further pre-requisites.

## Role Variables

```yaml
zammad_domain_name: "{{ ansible_fqdn }}"
```
Zammad's fully qualified domain name.

```yaml
zammad_nginx_config_path: "/etc/nginx/sites-available/zammad.conf"
```
File path to Zammad's Nginx config.

```yaml
zammad_ssl_cert_path: "/etc/ssl/certs/zammad_cert.pem"
```
File path to the SSL/TLS certificate which is used for HTTPS.

```yaml
zammad_ssl_key_path: "/etc/ssl/private/zammad_key.pem"
```
File path to the SSL/TLS private key  which is used for HTTPS.

```yaml
zammad_ssl_cert:
```
Content of SSL/TLS certificate.

```yaml
zammad_ssl_key:
```
Content of SSL/TLS private key.

## Dependencies

Zammad requires Elasticsearch and PostgreSQL database server:
- Elasticsearch - [elastic.elasticsearch](https://galaxy.ansible.com/elastic/elasticsearch)
- PostgreSQL - [geerlingguy.postgresql](https://galaxy.ansible.com/geerlingguy/postgresql)

## Example Playbook

```yaml
    - hosts: servers
      roles:
         - role: ufz.zammad
           become: yes
```

## License

MIT

## Author Information

This role was created in 2020 by [HIFIS Software Services](https://software.hifis.net/).
