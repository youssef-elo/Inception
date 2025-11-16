FROM debian:bookworm

RUN apt-get update && apt-get install -y nginx

COPY nginx.conf /etc/nginx/nginx.conf


#the reason for the -g daemon off flags is so the nginx process doesnt fork itself 
#and run in the backgroun since that is the default behavior for nginx, 
#and since it is ran in a container if the main process ( pid 1 ) exits 
#the container will be deemed as fininshed so it will be stoped
CMD ["nginx" , "-g" ,"daemon off;"]
