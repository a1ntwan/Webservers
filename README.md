First of all, if you want everything to be fine, you do definitely need to:

1. Turn off or set to permissive SElinux/apparmor;
2. Turn off or allow required ports in your firewall settings;
3. Make sure you time is synchronized on all of you nodes;
4. Your locale settings are configured properly.


These are 4 implementations of **Nginx + backend + database**:
***
1) Nginx + Gunicorn + Postgresql
2) Nginx + PHP-FPM8 + MySQL/MariaDB
3) Nginx + Wordpress and PHP-FPM8 + MySQL/MariaDB
4) Nginx + Node.js + MongoDB
***

You may need extra ansible-galaxy collection to work with certificates:
```
ansible-galaxy collection install community.crypto
```
These playbooks have been tested on **Centos7** and **Ubuntu 20.04**.