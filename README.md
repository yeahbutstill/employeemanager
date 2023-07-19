# employeemanager
App to manage employees

## Setup Docker for MySQL
```shell
docker run --rm \
--name=employeemanager-db \
-e MYSQL_DATABASE=employeemanager \
-e MYSQL_USER=employeemanager \
-e MYSQL_PASSWORD=PNSJkxXvVNDAhePMuExTBuRR \
-e MYSQL_ROOT_PASSWORD=PNSJkxXvVNDAhePMuExTBuRR \
-e TZ=Asia/Jakarta \
-p 6603:3306 \
-v "$PWD/docker/employeemanager-db/conf.d":/etc/mysql/conf.d \
-v "$PWD/storage/docker/employeemanagerdb-data":/var/lib/mysql \
mysql:8
```