# PRTIMES_intern

https://github.com/catatsuy/private-isu
に挑戦してみる。

## docker起動方法
```
docker-compose build
docker-compose up
```

## mySQLログイン
```
docker exec -it webapp_mysql_1  bash
SQL> mysql -u root -p
```

## ベンチマーク起動
```
docker run --network host -i private-isu-benchmarker //opt/go/bin/benchmarker -t http://host.docker.internal -u //opt/go/userdata
```
