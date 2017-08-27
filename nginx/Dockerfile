FROM nginx:1.12.1
MAINTAINER juliansalas080@gmail.com

#Crea la sites-enable
RUN mkdir /etc/nginx/sites-enabled

# Se hace copy de los sitios enables
COPY /sites-available/*.conf /etc/nginx/sites-available/
RUN  ln -s /etc/nginx/sites-available/*  /etc/nginx/sites-enabled/


# Copy data source from parent directory
COPY democracia /www/data/democracy
COPY nginx.conf /etc/nginx/nginx.conf
RUN chown -R nginx:nginx /www 

RUN mkdir /www/data/democracy/app
RUN chown -R nginx:nginx /www/data/democracy/app

