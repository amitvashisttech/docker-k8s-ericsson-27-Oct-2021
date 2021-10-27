# Base Image
FROM ubuntu:16.04

# Owner of Image
MAINTAINER Amit Vashist <amitvashist7@outlook.com>

# Update the APT-REPO
RUN apt-get update

# Install Apache Packages 
RUN apt-get install apache2 -y

# Deploy Custom Web Page
COPY index.html /var/www/html/ 

# Expose 80
EXPOSE 80

# Excute the Apache Process
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]

