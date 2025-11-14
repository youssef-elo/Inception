FROM debian:bookworm

RUN apt-get update && apt-get install -y nginx

COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 9090

CMD ["nginx" , "-g" ,"daemon off;"]