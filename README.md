# kafka-mybatis-plus-template
 ```
本项目是基于springkafka项目 
实现的主要目标
 1、可以自定义管理topic及消费端的动态配置
 2、可以启动、停止消费客户端

  项目数据库目前用的是mysql所以需要先创建数据库和表。 修改配置文件 application.yml 中的数据库连接信息，然后执行下面 sql 创建 database: 
  CREATE DATABASE IF NOT EXISTS kafka_config CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
  确保数据库连接正确后，由于项目使用了 Liquibase 进行数据库初始化和更新，所以只需要启动项目即可。
```
