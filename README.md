# Custom Courseware Dev Setup

### Setup
1. Configure DNS
*.test domains need to resolve to localhost.


You can the following FQDN to your /etc/hosts file:
- ui.custom-courseware.test
- api.custom-courseware.test
- keycloak.custom-courseware.test


Or you can use a secondary DNS service.
I use the following [ansible script](https://github.com/JamesAyres16/ansible/blob/main/local-setup/dns-for-test.yml)
for my test setup.


2. Start containers
``` bash
docker compose up
sudo docker compose up -f docker-compose.dns.yml
```
