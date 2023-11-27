# 数据库

整理了一些常用的数据库相关资料、笔记与操作手册

公网资料、笔记地址请访问这里 


<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->

<!-- PROJECT LOGO -->

--------------------

## 基本概念

数据库（Database）是用于存储、管理、检索和操作数据的系统。它通过组织和存储数据使得我们能够高效地访问和管理数据。数据库通常由数据库管理系统（DBMS）来操控，通过DBMS，用户可以执行数据的创建、读取、更新和删除（CRUD）操作。

### 数据库可以大致分类为以下几种类型
+ 关系型数据库（RDBMS）：以表格形式存储数据，每个表格被称为关系。它们通过公共字段将不同的表连接起来。关系型数据库使用结构化查询语言（SQL）进行数据操作。典型的关系型数据库包括MySQL、PostgreSQL、Oracle、Microsoft SQL Server等。
+ 非关系型数据库（NoSQL）：与关系型数据库相比，非关系型数据库对于不需要严格结构的数据来说更为灵活。它们可以存储半结构化数据或非结构化数据，并以各种方式组织数据，如键-值对、列存储、文档存储、图数据库等。著名的NoSQL数据库包括MongoDB、Cassandra、Redis、Neo4j等。
+ 对象数据库：存储面向对象编程语言中的对象实例，允许复杂数据对象被直接存储。比较少见，主要用于特殊行业或领域。
+ 分布式数据库：分布在多个物理位置的数据集合，可以分散在同一个网络、跨多个数据中心。它们旨在提供高可用性和分区容错。

### 数据库的主要特点包括
+ 数据的持久性：数据在数据库中长期存储，即使系统关闭，数据也不会消失。
+ 原子性：数据库更新操作要么完全执行，要么完全不执行，确保数据的一致性。
+ 并发控制：多用户可以同时访问数据库，DBMS需要确保数据的一致性和完整性。
+ 安全性：数据库利用访问控制和加密来保证数据的安全性。
+ 备份与恢复：数据库支持数据备份和在发生故障时恢复的功能。

--------------------

## 目录

[目录](index.md)

## Mysql

### 参考文档
[Mysql5.7 参考手册](Mysql/资料/MySQL 5.7 参考手册.pdf)

[第01章_数据库概述](Mysql/课件/第01章_数据库概述.pdf)

[第02章_MySQL环境搭建](Mysql/课件/第02章_MySQL环境搭建.pdf)

[第03章_基本的SELECT语句](Mysql/课件/第03章_基本的SELECT语句.pdf)

[第04章_运算符](Mysql/课件/第04章_运算符.pdf)

[第05章_排序与分页](Mysql/课件/第05章_排序与分页.pdf)

[第06章_多表查询](Mysql/课件/第06章_多表查询.pdf)

[第07章_单行函数](Mysql/课件/第07章_单行函数.pdf)

[第08章_聚合函数](Mysql/课件/第08章_聚合函数.pdf)

[第09章_子查询](Mysql/课件/第09章_子查询.pdf)

[第10章_创建和管理表](Mysql/课件/第10章_创建和管理表.pdf)

[第11章_数据处理之增删改](Mysql/课件/第11章_数据处理之增删改.pdf)

[第12章_MySQL数据类型精讲](Mysql/课件/第12章_MySQL数据类型精讲.pdf)

[第13章_约束](Mysql/课件/第13章_约束.pdf)

[第14章_视图](Mysql/课件/第14章_视图.pdf)

[第15章_存储过程与函数](Mysql/课件/第15章_存储过程与函数.pdf)

[第16章_变量、流程控制与游标](Mysql/课件/第16章_变量、流程控制与游标.pdf)

[第17章_触发器](Mysql/课件/第17章_触发器.pdf)

[第18章_MySQL8其它新特性](Mysql/课件/第18章_MySQL8其它新特性.pdf)


## Oracle

### 参考文档

[Oracle11g官方文档中英对照版_pdf](Oracle/pdf/Oracle11g官方文档中英对照版.pdf)

[基本语法与定义_pdf](Oracle/pdf/ORACLE九阴真经.pdf)

[oracle原理与白皮书_pdf](Oracle/pdf/oracle知识库.pdf)

[函数手册1_pdf](Oracle/pdf/oracle函数大全-分类显示.pdf)

[函数手册2_pdf](Oracle/pdf/Oracle函数大全.pdf)

[函数手册(官方)_pdf](Oracle/pdf/Oracle函数手册.pdf)

[SQL完整手册1_chm](Oracle/chm/Ora9iSQL参考手册.chm)

[SQL完整手册2_chm](Oracle/chm/SQL语言参考大全.chm)

[SQLCodes-Oracle错误代码与消息解释_chm](Oracle/chm/SQLCodes-Oracle错误代码与消息解释.chm)


## Neo4j

### 参考文档
[Neo4j详细笔记](Neo4j/neo4j.md)

[Neo4j官方手册](Neo4j/文档/neo4j-cypher-manual-4.3.pdf)

[Java对接手册](Neo4j/文档/neo4j-driver-manual-4.3-java.pdf)

[Java对接补充](Neo4j/文档/neo4j-java-reference-4.3.pdf)


## MongoDB

### 参考文档
[中文在线文档](https://docs.whaleal.com/mongodb-manual-zh/docs/#)


## RABC

### 参考文档

[简易mysql示例](./RBAC.md)


## 贡献者

请阅读**CONTRIBUTING.md** 查阅为该项目做出贡献的开发者。

#### 如何参与开源项目

贡献使开源社区成为一个学习、激励和创造的绝佳场所。你所作的任何贡献都是**非常感谢**的。


1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 版本控制

该项目使用Git进行版本管理。您可以在repository参看当前可用版本。

<!-- ## 作者 -->
<!--  -->
<!-- [小昊子](https://github.com/worst001) -->
<!--  -->
<!-- 制做不易，如果有帮到你就请作者喝杯咖啡吧! -->
<!--  -->
<!-- ![支付宝加微信](https://xiyou-oss.oss-cn-shanghai.aliyuncs.com/%E5%85%AC%E4%BC%97%E5%8F%B7%E4%B8%8E%E6%94%AF%E4%BB%98/%E6%94%AF%E4%BB%98%E5%AE%9D%E5%8A%A0%E5%BE%AE%E4%BF%A1.jpg) -->
<!--  -->
<!-- 作者无聊时做的测试游戏，完全免费哦！ -->
<!--  -->
<!-- ![公众号](https://xiyou-oss.oss-cn-shanghai.aliyuncs.com/%E5%85%AC%E4%BC%97%E5%8F%B7%E4%B8%8E%E6%94%AF%E4%BB%98/%E5%85%AC%E4%BC%97%E5%8F%B7%E5%B0%8F.jpg) -->

## 参考资料

[尚硅谷系列教程资料](http://www.atguigu.com/opensource.shtml)

<!-- links -->
[your-project-path]:shaojintian/Best_README_template
[contributors-shield]: https://img.shields.io/github/contributors/worst001/mkdocs_db.svg?style=flat-square
[contributors-url]: https://github.com/worst001/mkdocs_db/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/worst001/mkdocs_db.svg?style=flat-square
[forks-url]: https://github.com/worst001/mkdocs_db/network/members
[stars-shield]: https://img.shields.io/github/stars/worst001/mkdocs_db.svg?style=flat-square
[stars-url]: https://github.com/worst001/mkdocs_db/stargazers
[issues-shield]: https://img.shields.io/github/issues/worst001/mkdocs_db.svg?style=flat-square
[issues-url]: https://img.shields.io/github/issues/worst001/mkdocs_db.svg
[license-shield]: https://img.shields.io/github/license/worst001/mkdocs_db.svg?style=flat-square
[license-url]: https://github.com/worst001/mkdocs_db/blob/main/LICENSE.txt
<!-- [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555 -->
<!-- [linkedin-url]: https://linkedin.com/in/shaojintian -->
