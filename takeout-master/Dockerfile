# 使用官方的 Nginx 镜像作为基础镜像
FROM nginx:latest

# 复制自定义的 Nginx 配置文件到容器中
COPY ./etc/nginx/nginx.conf /etc/nginx/nginx.conf

# 复制站点文件到容器中
COPY ./takeout-master/backend/src/main/resources/static/index.html

# 暴露端口
EXPOSE 80

# 启动 Nginx 服务
CMD ["nginx", "-g", "daemon off;"]
