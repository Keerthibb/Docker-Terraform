FROM ubuntu

RUN apt-get update && apt-get install apache2 -y
EXPOSE 80

ENTRYPOINT service apache2 start && /bin/bash
VOLUME C:\Users\kbb\Downloads\Docker_hub:/apache_data
WORKDIR /PDN
COPY index.html /var/www/html/index.html