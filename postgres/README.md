# 特点

* 安装PostGIS 2.5

# 运行示例

```
$ docker run -d --restart=always \
-v ${PWD}/postgres:/data \
-p 65432:5432 \
-e PGDATA=/data -e TZ=Asia/Shanghai -e POSTGRES_PASSWORD=any_password \
--name "postgres" xm69/postgres:12-gis2.5
```

# 构建

```
$ docker build -t xm69/postgres:12-gis2.5 .
```
