FROM amazoncorretto:17-alpine3.18-jdk

LABEL maintainer="Longjianghu <215241062@qq.com>"

# 更换源
RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories && apk update

# 时区设置
RUN apk add --no-cache tzdata fontconfig ttf-dejavu font-terminus

ENV TIMEZONE="Asia/Shanghai"
RUN ln -snf /usr/share/zoneinfo/${TIMEZONE} /etc/localtime && echo ${TIMEZONE} > /etc/timezone