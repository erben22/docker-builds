# Version: 0.0.1
FROM ubuntu:16.04
MAINTAINER R. Cody Erben "erben22@mtnaircomputer.net"
ENV REFRESHED_AT 2016-02-01

RUN apt-get update && apt-get install -y nginx

# Alternate form we could use if a shell is not available:
#RUN [ "apt-get", " install", "-y", "nginx" ]

RUN echo 'Hi, I am in your container' \
    >/usr/share/nginx/html/index.html
EXPOSE 80

#CMD [ "/bin/bash" ]
#ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]

ENTRYPOINT ["/usr/sbin/nginx"]
CMD ["-h"]

LABEL version="0.1"
LABEL location="Boise" type="Test Container" role="Web Server"
