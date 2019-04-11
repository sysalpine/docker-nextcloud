# Custom Nextcloud Docker Images

## Images

* nextcloud-fpm (`based on fpm (-alpine) image with some custom php variables`)
* nextcloud-web (`nginx web server as proxy`)

### nextcloud-fpm

Use with docker compose files

```yml
[...]
  environment:
    PHP_MEMORY_LIMIT: "1G"
```
