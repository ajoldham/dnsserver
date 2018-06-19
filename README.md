Docker DNS Server
=================

This installs Ubuntu 16.04 running a BIND 9 DNS Server.

Build with:
```php
docker build -t dnsserver .
```

To map the current directory to the DNS server run with:
```php
docker-compose up
```

Configure with the following.  Some sample entries for 192.168.123.x have been created.
```php
https://127.0.0.1:10000
Username: root
Password: password
```

Note:  You may need to disable/allow a local firewall to receive UDP 53 DNS requests in Docker.
