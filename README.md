# Custom Nextcloud Docker Images

## Images

* nextcloud-fpm (`based on fpm (-alpine) image with some custom php variables`)
* nextcloud-web (`nginx web server as proxy`)

### nextcloud-fpm

Based on the official nextcloud-fpm docker image (<https://github.com/nextcloud/docker/>) with some customizations.

```yml
[...]
  environment:
    PHP_MEMORY_LIMIT: "1G"
```

### nextcloud-web

Nginx proxy image