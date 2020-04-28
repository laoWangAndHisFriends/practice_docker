FROM ubuntu:latest
WORKDIR /root

COPY ./config /root/.ssh/config
COPY ./known_hosts /root/.ssh/known_hosts
COPY ./2654189525@qq.com /root/.ssh/2654189525@qq.com

COPY ./sources.list /etc/apt/sources.list
COPY ./install_oh_my_zsh.sh /root/install_oh_my_zsh.sh

COPY ./install_nvm.sh /root/install_nvm.sh

RUN apt-get update && apt-get install zsh git -y && chmod +x /root/install_oh_my_zsh.sh && /root/install_oh_my_zsh.sh && chmod +x /root/install_nvm.sh && /root/install_nvm.sh && apt-get install vim pdfgrep ghostscript gcc make -y
RUN mkdir playground workspace tools && chmod 600 /root/.ssh/* &&  git config --global user.email 2654189525@qq.com && git config --global user.name wangkaixuan 
RUN cd playground && git clone git@github.com:iroan/practice_c.git && git clone git@github.com:iroan/practice_cpp.git && git clone git@github.com:iroan/practice_js.git && git clone git@github.com:iroan/practice_node.git && git clone git@github.com:iroan/practice_go.git  && git clone git@github.com:iroan/practice_py.git && git clone git@github.com:iroan/practice_shell.git && git clone git@github.com:iroan/linux_config.git && mv /root/playground/linux_config/* /root/
# https://nodejs.org/dist/v12.16.3/node-v12.16.3-linux-x64.tar.xz
# https://dl.google.com/go/go1.14.2.linux-amd64.tar.gz
# https://www.python.org/ftp/python/3.8.2/Python-3.8.2.tgz