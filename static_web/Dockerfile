# version 0.0.1
FROM ubuntu:14.04
LABEL DC Morrison "nosirromd@gmail.com"
RUN apt-get update
RUN ["apt-get", "install",  "-y", "nginx"]
RUN echo 'Hi, I am in DC Morrison''s container' \
    >/usr/share/nginx/html/index.html
EXPOSE 80
ENTRYPOINT ["/usr/sbin/nginx"]
CMD ["-h"]
VOLUME [ "/data" ]


