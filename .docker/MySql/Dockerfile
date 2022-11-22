# ベースとなるDockerイメージ指定
FROM mysql:8.0

RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && chown -R mysql:root /var/lib/mysql/

COPY ./DB/conf.d /etc/mysql/conf.d
COPY ./SQL/docker-entrypoint-initdb.d /docker-entrypoint-initdb.d

EXPOSE 3306
