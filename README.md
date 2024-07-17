# kafka-mybatis-plus-eki 项目介绍

## 项目概述

`kafka-mybatis-plus-eki` 是一个基于 Spring 和 emq-kafka-integration   自定义组件高级应用，它旨在提供一个灵活且易于管理的 Kafka 消费者和配置管理工具，此应用的主要目标主要是为了如何使用emq-kafka-integration自定义组件。

## 主要实现目标

1. **自定义管理Topic及消费端动态配置**：通过项目提供的接口或管理工具，允许用户自定义管理 Kafka 的 Topic 及其消费端的动态配置。
2. **启动、停止消费客户端**：提供API或管理工具，允许用户动态地启动或停止 Kafka 的消费客户端。

## 数据库设置

### 创建数据库和表

项目使用 MySQL 作为数据库，需要先创建一个名为 `kafka_config` 的数据库。你可以使用以下 SQL 语句来创建数据库（确保已连接到 MySQL）：

``` 
CREATE DATABASE IF NOT EXISTS kafka_config CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```
## 注意事项

项目使用 Liquibase 进行数据库的初始化和更新。在启动项目后，Liquibase 会自动执行必要的数据库变更脚本，创建或更新必要的表结构。
