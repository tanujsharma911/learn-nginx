# Learn Nginx

1. Install
```
sudo apt update
sudo apt install nginx
```

2. Check if Nginx is running
```
sudo systemctl status nginx
```
```
curl http://localhost
```

3. Installation location
```
whereis nginx
```
#### output:
```
nginx: /usr/sbin/nginx /etc/nginx /usr/share/nginx /usr/share/man/man8/nginx.8.gz
```

4. Important files and folders structure
```
/etc/nginx
├── nginx.conf
├── site-available
├── site-enabled
└── conf.d
```

5. **nginx.conf** sample code
```
events {}
http {
        include /etc/nginx/mime.types;
        include /etc/nginx/sites-enabled/*;
}
```

6. sites-enabled folder
```
root@/etc/nginx/sites-enabled 👉 ls -la /etc/nginx/sites-enabled
total 8
drwxr-xr-x 2 root root 4096 Jun 23 09:12 .
drwxr-xr-x 8 root root 4096 Jul  1 01:21 ..
lrwxrwxrwx 1 root root   37 Feb 25 14:14 chesskhelo         -> /etc/nginx/sites-available/chesskhelo
lrwxrwxrwx 1 root root   32 Jun  8 14:17 cotex              -> /etc/nginx/sites-available/cotex
lrwxrwxrwx 1 root root   45 Feb 25 14:14 snakes_and_ladders -> /etc/nginx/sites-available/snakes_and_ladders
```