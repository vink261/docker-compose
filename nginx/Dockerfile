FROM centos:7

MAINTAINER Vinh

# Install epel repository
RUN yum install -y http://dl.fedoraproject.org/pub/epel/6/i386/epel-release-6-8.noarch.rpm && yum update -y && yum clean all -y

# Install nginx
RUN yum install -y nginx

# Remove the default nginx configuration file
RUN rm -v /etc/nginx/nginx.conf

# Copy a configuration file from the current directory
# ADD logs/nginx /var/log/nginx
# ADD nginx/nginx_conf /etc/

# Append "daemon off;" to the beginning of the configuration
RUN echo "daemon off;" >> /etc/nginx/nginx.conf

CMD service nginx start