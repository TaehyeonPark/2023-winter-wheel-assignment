FROM nginx:1.18.0

COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./sites-enabled /etc/nginx/sites-enabled
COPY ./sites-available /etc/nginx/sites-available
COPY /etc/letsencrypt/live/taxi.taehyeon.me /etc/letsencrypt/live/taxi.taehyeon.me

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]