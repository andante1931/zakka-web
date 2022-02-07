FROM mysql/mysql-server:8.0

ENV MYSQL_DATABASE=laravel_local \
  MYSQL_USER=phper \
  MYSQL_PASSWORD=secret \
  MYSQL_ROOT_PASSWORD=secret \
  TZ=Asia/Tokyo

# mysqlの設定ファイルを指定
COPY ./my.cnf /etc/my.cnf
#　書き込み権限が付くとMySQLの起動時にエラーが発生する際の対応
RUN chmod 644 /etc/my.cnf
