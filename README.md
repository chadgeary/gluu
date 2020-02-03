# Reference
Installation of the Gluu service on Centos 7 (or RHEL7) with a LetsEncrypt-signed certificate and autorenewal cron.

# Requires
- port 80 open for certbot
- DNS resolution of friendly_name to instance public address

# Deployment
```
ansible-playbook gluu.yml --extra-vars "target=localhost friendly_name=sso.chadg.net domain_name=chadg.net certbot_email=chad@chadg.net"
```

# Todo
- wait for gluu-server-setup to complete
