FROM debian:Bookworm

RUN apt-get update && apt-get install nginx

COPY nginx.conf /etc/nginx/conf.d/nginx.conf

ENTRYPOINT [ "nginx", "-g", "daemon off"]