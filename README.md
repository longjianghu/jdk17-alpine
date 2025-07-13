### 项目说明

JDK17 运行基础镜像,基于amazoncorretto:17-alpine3.18-jdk镜像，更改时区为上海。


### 构建容器

docker build -t longjianghu/jdk:17 ./

### Docker 镜像

docker pull longjianghu/jdk:17