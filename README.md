Examle of chive installing for CentOS
======================

Create dirs and install chive:

```bash
mkdir /var/www/chive && cd $_ && wget -O - http://www.chive-project.com/Download/Redirect | tar -xzp && mkdir logs && mv chive public && wget -P public http://www.chive-project.com/favicon.ico
```

Copy config:

```bash
wget -P /etc/nginx/conf.d https://raw.githubusercontent.com/Webtoucher/chive-nginx-config/master/chive.conf
```

Fix downloaded config: change hostname and choose your FastCGI listener
