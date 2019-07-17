FROM golang:latest
LABEL author="wangkaixuan"
LABEL email="iroanuc@gmail.com"
RUN export GOPROXY="https://goproxy.io"
RUN go get -v -u github.com/astaxie/beego
RUN go get -v -u github.com/beego/bee
RUN go get -v -u github.com/go-sql-driver/mysql
RUN go get -v -u github.com/smartystreets/goconvey/convey