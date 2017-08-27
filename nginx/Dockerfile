FROM nginx:1.12.1
MAINTAINER juliansalas080@gmail.com


# Copy data source from parent directory
COPY democracia /www/data/democracy
COPY nginx.conf /etc/nginx/nginx.conf
RUN chown -R nginx:nginx /www 


