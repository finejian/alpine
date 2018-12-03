FROM golang:1.11.2-alpine3.7
RUN apk --no-cache add gcc g++ make ca-certificates tzdata openssh sshpass \
    && update-ca-certificates 2>/dev/null || true \
    && cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && echo "Asia/Shanghai" > /etc/timezone \
    && apk del tzdata
