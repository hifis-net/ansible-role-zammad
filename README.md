# Ansible role: Zammad
![](https://github.com/Helmholtz-UFZ/ansible-role-zammad/workflows/CI/badge.svg)

An Ansible Role that installs Zammad on Linux.

**Note:** This role does not install elasticsearch  and postgresql server. See 
[Dependencies](#dependencies).
## Requirements
The below requirements are needed on the target host:
- PyOpenSSL >= 0.15 or cryptography >= 1.2.3

## Role Variables

```yaml
zammad_version: "3.3.0"
```
Zammad version to be installed.

```yaml
zammad_release_channel: "stable"
```
Choose another release channel for the Zammad packages.
Please refer to https://packager.io/gh/zammad/zammad for a complete list.

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
Content of SSL/TLS certificate (**required**).

```yaml
zammad_ssl_key:
```
Content of SSL/TLS private key (**required**).

```yaml
zammad_nginx_server_tokens: "off"
```
Enable or disable emitting nginx version information in error pages or in the
_Server_ response header field. Please read the nginx
[docs](http://nginx.org/en/docs/http/ngx_http_core_module.html#server_tokens)
for further information.

```yaml
zammad_nginx_additional_server_configs:
  - |
      server {
        listen 80;
        server_name zammad.example.com zammad-old.example.com;
        return 301 https://zammad.example.com$request_uri;
      }
  - |
      server {
        listen 443 ssl;

        # ... SSL configuration

        server_name zammad-old.example.com;
        return 301 https://zammad.example.com$request_uri;
      }
```
Configure additional server directives in the Nginx configuration.
This allows to implement more use case specific adjustments, e.g.
configuring multiple domains or the redirection of outdated domains to the
most recent one.

```yaml
elasticsearch_url: "http://localhost:9200"
```
Elasticsearch server address.

## Dependencies

Zammad requires Elasticsearch and PostgreSQL database server. This role has
been successfully tested together with the following roles: 
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
