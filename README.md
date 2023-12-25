<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->

<!-- PROJECT LOGO -->

<!-- 项目LOGO -->
<br />
<div align="center">
  <a href="http://mkdocs.grft.top">
    <img src="https://xiyou-oss.oss-cn-shanghai.aliyuncs.com/mkdocs/logo.png" alt="Logo" width="480" height="270">
  </a>

  <h3 align="center">数据库</h3>

  <p align="center">
    <br />
    <a href="http://mkdocs.grft.top/数据库/"><strong>探索文档 »</strong></a>
    <br />
  </p>
</div>

<!-- 目录 -->
<details>
  <summary>目录</summary>
  <ol>
    <li><a href="#关于项目">关于项目</a></li>
    <li><a href="#什么是数据库">什么是数据库</a></li>
    <li><a href="#技术目录">技术目录</a></li>
    <li><a href="#贡献">贡献</a></li>
    <li><a href="#许可证">许可证</a></li>
    <li><a href="#联系方式">联系方式</a></li>
    <li><a href="#鸣谢">鸣谢</a></li>
  </ol>
</details>


## 关于项目

整理了一些常用的数据库相关资料、笔记与操作手册

公网资料、笔记地址请访问这里 

- 文档地址: [http://mkdocs.grft.top/数据库/](http://mkdocs.grft.top/数据库/)

其他相关技术可以访问我的博客，主页地址请访问这里

- 访问入口：[http://mkdocs.grft.top](http://mkdocs.grft.top)

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

## 什么是数据库

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

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

## 技术目录

[目录与大纲](index.md)

### Mysql

+ [Mysql5.7 参考手册](Mysql/资料/MySQL-5.7_参考手册.pdf)

#### 尚硅谷课件资料

+ [第01章_数据库概述](Mysql/课件/第01章_数据库概述.pdf)
+ [第02章_MySQL环境搭建](Mysql/课件/第02章_MySQL环境搭建.pdf)
+ [第03章_基本的SELECT语句](Mysql/课件/第03章_基本的SELECT语句.pdf)
+ [第04章_运算符](Mysql/课件/第04章_运算符.pdf)
+ [第05章_排序与分页](Mysql/课件/第05章_排序与分页.pdf)
+ [第06章_多表查询](Mysql/课件/第06章_多表查询.pdf)
+ [第07章_单行函数](Mysql/课件/第07章_单行函数.pdf)
+ [第08章_聚合函数](Mysql/课件/第08章_聚合函数.pdf)
+ [第09章_子查询](Mysql/课件/第09章_子查询.pdf)
+ [第10章_创建和管理表](Mysql/课件/第10章_创建和管理表.pdf)
+ [第11章_数据处理之增删改](Mysql/课件/第11章_数据处理之增删改.pdf)
+ [第12章_MySQL数据类型精讲](Mysql/课件/第12章_MySQL数据类型精讲.pdf)
+ [第13章_约束](Mysql/课件/第13章_约束.pdf)
+ [第14章_视图](Mysql/课件/第14章_视图.pdf)
+ [第15章_存储过程与函数](Mysql/课件/第15章_存储过程与函数.pdf)
+ [第16章_变量、流程控制与游标](Mysql/课件/第16章_变量、流程控制与游标.pdf)
+ [第17章_触发器](Mysql/课件/第17章_触发器.pdf)
+ [第18章_MySQL8其它新特性](Mysql/课件/第18章_MySQL8其它新特性.pdf)

#### 详细笔记

+ [数据类型](Mysql/详细笔记/数据类型.md)
+ [语法](Mysql/详细笔记/语法.md)
+ [MySQL常用函数汇总](Mysql/详细笔记/MySQL常用函数汇总.md)
+ [MySQL数据库开发三十六条军规](Mysql/详细笔记/MySQL数据库开发的三十六条军规.md)
+ [MySQL数据库设计规范](Mysql/详细笔记/MySQL数据库设计规范.md)

### Oracle
+ [Oracle11g官方文档中英对照版_pdf](Oracle/pdf/Oracle11g官方文档中英对照版.pdf)
+ [基本语法与定义_pdf](Oracle/pdf/ORACLE九阴真经.pdf)
+ [oracle原理与白皮书_pdf](Oracle/pdf/oracle知识库.pdf)
+ [函数手册1_pdf](Oracle/pdf/oracle函数大全-分类显示.pdf)
+ [函数手册2_pdf](Oracle/pdf/Oracle函数大全.pdf)
+ [函数手册(官方)_pdf](Oracle/pdf/Oracle函数手册.pdf)
+ [SQL完整手册1_chm](Oracle/chm/Ora9iSQL参考手册.chm)
+ [SQL完整手册2_chm](Oracle/chm/SQL语言参考大全.chm)
+ [SQLCodes-Oracle错误代码与消息解释_chm](Oracle/chm/SQLCodes-Oracle错误代码与消息解释.chm)


### Neo4j

+ [Neo4j详细笔记](Neo4j/neo4j.md)
+ [Neo4j官方手册](Neo4j/文档/neo4j-cypher-manual-4.3.pdf)
+ [Java对接手册](Neo4j/文档/neo4j-driver-manual-4.3-java.pdf)
+ [Java对接补充](Neo4j/文档/neo4j-java-reference-4.3.pdf)


### MongoDB

+ [中文在线文档](https://docs.whaleal.com/mongodb-manual-zh/docs/#)
+ [技术索引手册](MongoDB/README.md)


### RABC

+ [Mysql版简易示例](RBAC.md)

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

<!-- 贡献 -->

## 贡献

贡献是使开源社区成为一个如此令人惊叹的地方，以学习、激励和创造。您所做的任何贡献都将非常感谢。

如果您对使这个项目变得更好有建议，请 fork 该仓库并创建 pull request。您也可以打开一个带有“enhancement”标签的问题。不要忘记给这个项目点个星！再次感谢！

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>


<!-- 许可证 -->
## 许可证

根据 MIT 许可证进行分发。更多信息请参见 [LICENSE.txt](LICENSE)。

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

<!-- 联系方式 -->
## 联系方式

关注我: [小昊子](https://github.com/worst001)

博客地址: [http://mkdocs.grft.top](http://mkdocs.grft.top)

项目链接: [https://github.com/worst001/mkdocs_db](https://github.com/worst001/mkdocs_db)

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

## 鸣谢

因为仓库与文档的数量比较大，有些借鉴资料忘了在`参考文档`部分提及原作者与原仓库，若有疏漏请告诉，我及时补上。

所有引用的原资料都确认是开源认证，若有侵权请告知。

[https://docs.whaleal.com](https://docs.whaleal.com)

[https://github.com/guanguans/notes](https://github.com/guanguans/notes)

[https://www.cnblogs.com/andy6/p/5723881.html](https://www.cnblogs.com/andy6/p/5723881.html)

[尚硅谷系列教程资料](http://www.atguigu.com/opensource.shtml)

[https://openai.com/chatgpt](https://openai.com/chatgpt)

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

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
