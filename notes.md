
1. Files and folders structure
```
/etc/nginx
├── nginx.conf
├── site-available
│   └── [PROJECT_NAME]
├── site-enabled
│   └── [PROJECT_NAME] -> /etc/nginx/sites-available/[PROJECT_NAME]
└── conf.d
```

2. Structure of blocks in **nginx.conf**
```
main
├── events
├── http
│   ├── server
│   │   └── location
│   └── upstream
├── stream
│   └── server   # TCP/UDP server
└── mail
    └── server   # Mail server
```

3. **nginx.conf** contains sample code of main config file

4. sites-enabled folder
```
root@/etc/nginx/sites-enabled 👉 ls -la /etc/nginx/sites-enabled
total 8
drwxr-xr-x 2 root root 4096 Jun 23 09:12 .
drwxr-xr-x 8 root root 4096 Jul  1 01:21 ..
lrwxrwxrwx 1 root root   37 Feb 25 14:14 chesskhelo         -> /etc/nginx/sites-available/chesskhelo
lrwxrwxrwx 1 root root   32 Jun  8 14:17 cotex              -> /etc/nginx/sites-available/cotex
lrwxrwxrwx 1 root root   45 Feb 25 14:14 snakes_and_ladders -> /etc/nginx/sites-available/snakes_and_ladders
```


