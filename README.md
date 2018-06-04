# Cetus

##  简介

Cetus是由C语言开发的关系型数据库MySQL的中间件，主要提供了一个全面的数据库访问代理功能。Cetus连接方式与MySQL基本兼容，应用程序几乎不用修改即可通过Cetus访问数据库，实现了数据库层的水平扩展和高可用。

## 主要功能特性

Cetus分为读写分离和分库两个版本。

|功能        						| 读写分离版本    |  分库版本 |
|- | :-: | -:|
|单进程无锁提升单个实例效率           | 支持      		|   支持    |
|支持透明的后端连接池        	    | 支持     		|   支持    |
|支持SQL读写分离       				| 支持      		|   不支持|
|增强SQL路由解析与注入       		| 支持      		|   不支持  |
|支持prepare语句       			| 支持      		|   不支持  |
|支持结果集压缩       				| 支持      		|   不支持  |
|支持安全性管理       				| 支持      		|   不支持  |
|支持状态监控       				| 支持      		|   不支持  |
|支持tcp stream流式       			| 支持      		|   不支持  |
|支持域名连接后端       			| 支持      		|   不支持  |
|SL/TLS支持       				| 支持      		|   不支持  |
|GR支持       					| 支持      		|   不支持  |
|读强一致性支持（待实现）       		| 待实现    		|   待实现  |
|支持数据分库       				| 不支持       	|   支持    |
|支持分布式事务处理       			| 不支持       	|   支持    |
|支持insert批量操作       			| 不支持       	|   支持    |
|支持有条件的distinct操作       	| 不支持       	|   支持    |
|具有性能优越的结果集合并算法     	| 不支持      	|   支持    |
|支持安全性管理       				| 不支持      	|   支持    |
|支持状态监控       				| 不支持      	|   支持    |
|支持tcp stream流式       			| 不支持     		|   支持    |


**针对读写分离版本：**

- 单进程无锁提升单个实例效率

- 支持透明的后端连接池

- 支持SQL读写分离

- 增强SQL路由解析与注入

- 支持prepare语句

- 支持结果集压缩

- 支持安全性管理

- 支持状态监控

- 支持tcp stream流式

- 支持域名连接后端

- SSL/TLS支持

- MGR支持

- 读强一致性支持（待实现）

**针对分库版本：**

- 单进程无锁提升单个实例效率

- 支持透明的后端连接池

- 支持数据分库

- 支持分布式事务处理

- 支持insert批量操作

- 支持有条件的distinct操作

- 增强SQL路由解析与注入

- 支持结果集压缩

- 具有性能优越的结果集合并算法

- 支持安全性管理

- 支持状态监控

- 支持tcp stream流式

- 支持域名连接后端

- SSL/TLS支持

- MGR支持

- 读强一致性支持（待实现）

## 详细说明

### Cetus安装与使用

1. [Cetus 快速入门](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-quick-try.md)

2. [Cetus 安装说明](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-install.md)

3. [Cetus 读写分离版配置文件说明](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-rw-profile.md)

4. [Cetus 分库(sharding)版配置文件说明](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-shard-profile.md)

5. [Cetus 启动配置选项说明](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-configuration.md)

6. [Cetus 使用约束说明](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-constraint.md)

7. [Cetus 读写分离版使用指南](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-rw.md)

8. [Cetus 读写分离版管理手册](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-rw-admin.md)

9. [Cetus 分库(sharding)版使用指南](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-sharding.md)

10. [Cetus 分库(sharding)版管理手册](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-shard-admin.md)

### Cetus架构与设计

[Cetus 架构和实现](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-architecture.md)

### Cetus发现的MySQL xa事务问题

[MySQL xa事务问题说明](https://github.com/Lede-Inc/cetus/blob/master/doc/mysql-xa-bug.md)

### Cetus辅助

1. [Cetus xa悬挂处理工具](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-xa.md)

2. [Cetus + mha高可用方案](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-mha.md)

3. [Cetus rpm说明](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-rpm.md)

### Cetus测试

[Cetus 测试报告](https://github.com/Lede-Inc/cetus/blob/master/doc/cetus-test.md)

## 反馈

如果您在使用Cetus的过程中发现BUG或者有新的功能需求，请加入QQ群(521824702)进行交流。
