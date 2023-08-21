FROM nginx:1.18.0

COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./sites-enabled /etc/nginx/sites-enabled
COPY ./sites-available /etc/nginx/sites-available

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]