# MySQL

MySQL由于其性能高、成本低、可靠性好，已经成为最流行的开源数据库，被广泛地应用在Internet上的中小型网站中。随着MySQL的不断成熟，它也逐渐用于更多大规模网站和应用，比如维基百科、Google和Facebook等网站。

本镜像源自于DockerHub镜像[mysql](https://registry.hub.docker.com/_/mysql/)。

## 版本

当前版本 MySQL 5.6.25

## 说明

容器启动后会自动创建一个具有所有权限的root用户，并根据环境变量${MYSQL\_ROOT\_PASSWORD}设置密码。

支持的环境变量如下：

- MYSQL\_ROOT\_PASSWORD，可选，root用户密码, 默认为root

- MYSQL_DATABASE，可选，容器启动后自动创建一个指定名字的数据库实例

- MYSQL_USER, MYSQL_PASSWORD，可选，为根据环境变量${MYSQL_DATABASE}创建的数据库实例创建一个有全部权限的用户

- MYSQL\_ALLOW\_EMPTY\_PASSWORD，可选，设置为*yes*即运行容器后允许root用户设置空白密码，该设置有安全风险，不建议使用



