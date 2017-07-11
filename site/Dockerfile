FROM library/alpine:latest

RUN set -x ; \
  getent group www-data || addgroup -g 82 -S www-data ; \
  id -u www-data &>/dev/null || adduser -u 82 -D -S -G www-data www-data && exit 0 ; exit 1
# 82 is the standard uid/gid for "www-data" in Alpine

RUN apk update && apk add nginx
ADD nginx.conf /etc/nginx/nginx.conf

RUN mkdir -p /var/www/site
RUN mkdir -p /run/nginx
ADD index.html /var/www/site/index.html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
