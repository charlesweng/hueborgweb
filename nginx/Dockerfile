FROM ubuntu

RUN apt-get update

RUN apt-get install nginx -y

COPY out/** /var/www/html/

COPY nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]