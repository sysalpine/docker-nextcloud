FROM nginx:1.17.4

LABEL description="Nextcloud nginx web server" \
      maintainer="SysAlpine <mail@sysalpine.com>"

ENV BACKEND_HOST=127.0.0.1 \
    BACKEND_PORT=9000

RUN apt-get update && apt-get install -y curl && apt-get clean

COPY nginx.conf /etc/nginx/nginx.conf
COPY entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]

