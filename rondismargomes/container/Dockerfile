# Based on Alpine 3.13
FROM alpine:3.13
RUN apk update

#LABEL
LABEL version="1.0" description="NGINXSRV" maintainer="Rondismar Gomes <rondismar@gmail.com>"

# Install NGINX.
RUN apk add --no-cache nginx

COPY index.html /var/www/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]