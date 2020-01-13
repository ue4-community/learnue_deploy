# Learnue 部署环境

## 目录结构

1. caddy 用来放 caddy 的证书
2. config/env.yml 填写后端配置,通过 volume 绑定到容器内
3. logs 后端日志
4. mysql_data 后端的数据库,通过 volume 绑定到容器内,便于备份
5. .env 配置 docker-compose.yml 中用到的环境变量
6. Caddyfile caddy 容器的代理配置,代理分别代理 docker-compose.yml 中的 web 服务
7. docker-compose.yml 容器编排
