# docker-mysql

* mysqlをDockerで起動する
* データの永続化を行う

## Component

```
kazuki@Kazuki-MacBook-Pro docker-mysql % tree
.
├── README.md
├── docker-compose.yml
└── mysql
    ├── Dockerfile
    ├── db
    │   └── (empty) # for data
    ├── initdb.d
    │   └── init.sql
    └── my.cnf
```

## Commands

```
docker-compose build
docker-compose up -d
docker-compose ps

docker exec -it mysql bash
# access as root user
mysql -u root -proot

# access as test user
mysql -u test -ptest
```

## Reference

* [Dockerで永続化したmySQLの環境を作る！](https://qiita.com/leafeon00000/items/e190cf92af3a487cc749)