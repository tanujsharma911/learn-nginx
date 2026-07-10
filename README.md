# Learn Nginx

### Basic Nginx Commands

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

4. Test Nginx configuration
```
nginx -t
```

5. Restart Nginx
```
systemctl restart nginx
```
```
nginx -s reload
```