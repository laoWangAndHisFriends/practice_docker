FROM ubuntu
MAINTAINER wangkaixuan 2654189525@qq.com
ADD ["sources.list","/etc/apt/sources.list"]
RUN mkdir wangkaixuan_practice_dockfile_demo1
RUN apt-get update
RUN apt-get install nginx -y
CMD ["/usr/sbin/nginx", "-g", "daemon off"];
EXPOSE 80

