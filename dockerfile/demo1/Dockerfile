FROM ubuntu
MAINTAINER wangkaixuan 2654189525@qq.com
RUN mkdir wangkaixuan_practice_dockfile_demo1
RUN sed -i 's/archive.ubuntu.com/mirrors.ustc.edu.cn/g' /etc/apt/sources.list
RUN sed -i 's/security.ubuntu.com/mirrors.ustc.edu.cn/g' /etc/apt/sources.list
RUN apt-get update
RUN apt-get install nginx -y
EXPOSE 80

