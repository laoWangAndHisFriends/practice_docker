# 目的
练习使用docker来封装nodejs应用

# 参考
- [把一个 Node.js web 应用程序给 Docker 化](https://nodejs.org/zh-cn/docs/guides/nodejs-docker-webapp/)

# 步骤
1. 准备好源代码
2. 构建镜像：`docker build -t wangkaixuan/node-web-app .`
3. 运行镜像，生成一个容器：`docker run -p 49160:8080 -d wangkaixuan/node-web-app`
4. 查看APP是否在运行：curl `url`