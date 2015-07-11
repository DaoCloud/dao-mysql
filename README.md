# MySQL

MySQL 借助于其性能高、成本低、可靠性好等优势已经成为当今最流行的开源数据库，被广泛地应用在各类中小型网站中。随着 MySQL 的不断成熟，它也逐渐用于更多大规模网站和应用，比如维基百科、Google 和 Facebook 等网站。

本镜像源自于 Docker Hub 镜像 **[mysql](https://registry.hub.docker.com/_/mysql/)**。

## 版本

当前版本 MySQL 5.6.25

## 说明

容器启动后会自动创建一个具有所有权限的 `root` 用户，并根据环境变量 `MYSQL_ROOT_PASSWORD` 设置密码。

支持的环境变量如下：

* `MYSQL_ROOT_PASSWORD`，`root` 用户的密码（可选，默认为 root）。

* `MYSQL_DATABASE`，容器启动后自动创建一个指定名字的数据库实例（可选）。

* `MYSQL_USER`，`MYSQL_PASSWORD`，为根据环境变量 `MYSQL_DATABASE` 创建的数据库实例创建一个有全部权限的用户（可选）。

* `MYSQL_ALLOW_EMPTY_PASSWORD`，设置为 `yes` 即运行容器后允许 `root` 用户使用空密码登录（可选）。

> 注意：允许 `root` 用户使用空密码登录存在严重的安全隐患，故不建议使用
