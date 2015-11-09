FROM nginx

# OS Update
ADD sources.list /etc/apt/sources.list
RUN apt-get update && apt-get -y install vim

# Nginx conf
ADD nginx.conf       /etc/nginx/
ADD fcgi.conf        /etc/nginx/
ADD servers.d/*.conf /etc/nginx/servers.d/

EXPOSE 80