1. Generate user
```
sh -c "echo -n 'user_name:' >> /etc/nginx/.htpasswd"
```

2. Check file created or not
```
cat /etc/nginx/.htpasswd
```

3. Generate password
```
sh -c "openssl passwd -apr1 >> /etc/nginx/.htpasswd"
```

Here `apr1` is algorithm