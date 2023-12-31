<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![Stargazers][stars-shield]][stars-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->

<!-- PROJECT LOGO -->

# 数据库

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

----------------------

## Mysql

### 参考文档

[Mysql5.7 参考手册](Mysql/资料/MySQL-5.7_参考手册.pdf)

[尚硅谷课件资料](Direction.md)

#### 详细笔记

[数据类型](Mysql/详细笔记/数据类型.md)

[语法](Mysql/详细笔记/语法.md)

[MySQL常用函数汇总](Mysql/详细笔记/MySQL常用函数汇总.md)

[MySQL数据库开发三十六条军规](Mysql/详细笔记/MySQL数据库开发的三十六条军规.md)

[MySQL数据库设计规范](Mysql/详细笔记/MySQL数据库设计规范.md)


### 基本介绍

MySQL是一种流行的开源关系型数据库管理系统（RDBMS），广泛应用于各种应用程序和网站开发中。

+ 关系型数据库：
    + MySQL是一个关系型数据库，数据以表格的形式进行组织和存储。每个表由列和行组成，使用结构化查询语言（SQL）进行操作和查询。
+ 可扩展性和性能：
    + MySQL具有良好的可扩展性，可以处理大规模的数据集和高并发访问。它支持主从复制、分区和集群等技术，以实现高可用性和性能优化。
+ 多用户并发访问：
    + MySQL支持多个用户同时访问数据库，并提供了事务支持，确保数据的一致性和完整性。通过锁机制和隔离级别设置，可以处理并发访问引起的数据冲突。
+ 安全性和权限控制：
    + MySQL提供了丰富的安全功能，包括用户身份验证、访问控制和加密传输。管理员可以控制用户对数据库的访问权限，并确保数据的安全性。
+ 存储过程和触发器：
    + MySQL支持存储过程和触发器的编写和执行。存储过程是一段预定义的代码块，可被重复调用；触发器是在数据库操作（如插入、更新、删除）前或后自动触发的动作。
+ 跨平台支持：
    + MySQL可以运行在多个操作系统上，包括Windows、Linux和macOS等。这使得它成为一个灵活和可移植的数据库解决方案。

----------

## Oracle

### 参考文档

[Oracle手册与资料汇总](Direction.md)

### 基本介绍
Oracle是一种强大而广泛使用的商业关系型数据库管理系统（RDBMS），由Oracle Corporation开发和提供。

+ 可靠性和稳定性：
    + Oracle以其卓越的可靠性而闻名，被广泛应用于企业级应用和关键业务系统。它具有高度的容错性、数据完整性和故障恢复机制，确保数据的安全和可用性。
+ 强大的功能集：
    + Oracle提供了丰富的功能和工具，用于数据管理、事务处理、并发控制、查询优化、安全性等方面。它支持ACID（原子性、一致性、隔离性、持久性）事务，并提供了强大的SQL查询和存储过程编程能力。
+ 可扩展性和性能：
    + Oracle具有良好的可扩展性，可以处理大规模数据集和高并发访问。它支持分布式数据库、水平分区和集群等技术，以实现高性能和高可用性。
+ 多用户并发访问：
    + Oracle支持多个用户同时访问数据库，并提供了强大的并发控制机制。通过锁机制、MVCC（多版本并发控制）和隔离级别设置，可以确保数据的一致性和隔离性。
+ 安全性和权限控制：
    + Oracle提供了广泛的安全功能，包括用户身份验证、访问控制、数据加密和审计等。管理员可以细粒度地控制用户对数据库对象和操作的权限。
+ 大量的工具和社区支持：
    + Oracle拥有庞大的用户社区和丰富的第三方工具支持。它提供了图形化管理工具（如Oracle Enterprise Manager）和开发工具（如SQL Developer），以及各种编程语言的Oracle驱动程序和API。


## Neo4j

### 参考文档
[Neo4j详细笔记](Neo4j/neo4j.md)

[Neo4j官方手册](Direction.md)

### 基本介绍
Neo4j是一种图形数据库管理系统，专注于存储和处理图形结构的数据。它使用图形模型来表示和处理数据，将实体（节点）之间的关系（边）作为重要的数据组织方式。

+ 图形数据库：
    + Neo4j是一种基于图形模型的数据库，用于存储和处理复杂的连接数据。图形模型以节点和边的形式表示数据，可以更自然地建模和查询关系型数据。
+ 节点和关系：
    + 在Neo4j中，数据被表示为节点和关系的集合。节点代表实体或对象，而关系表示节点之间的连接。节点和关系都可以包含属性，用于描述和扩展数据。
+ 灵活的查询语言：
    + Neo4j使用Cypher查询语言，提供了一种直观且易于理解的方式来查询和操作图形数据。Cypher语言类似于SQL，但专门针对图形数据模型进行优化。
+ 高性能：
    + 由于其图形数据结构和查询优化，Neo4j能够高效地处理大规模和高度连通的数据。它支持快速的节点和关系遍历，使得复杂的图形查询变得高效。
+ 灵活的数据模型：
    + 图形数据库的灵活性使得Neo4j适用于多种应用场景。它可以用于社交网络分析、推荐系统、知识图谱、网络和IT运维管理等领域。
+ 可扩展性：
    + Neo4j支持水平和垂直的扩展，以满足不断增长的数据需求。通过分布式部署和集群配置，可以实现高可用性和负载均衡。

## MongoDB

### 参考文档
[中文在线文档](https://docs.whaleal.com/mongodb-manual-zh/docs/#)

[技术索引手册](MongoDB/README.md)

### 基本介绍

MongoDB是一种开源的、面向文档的NoSQL数据库管理系统。

+ 文档数据库
    + MongoDB以文档的形式存储数据，文档是一个键值对的集合，类似于JSON格式。这种灵活的数据模型使得MongoDB适合处理半结构化和非结构化数据。
+ 可扩展性和高性能
    + MongoDB具有良好的可扩展性和高吞吐量的特点。它支持水平扩展，可以通过添加更多的服务器节点来处理大规模数据和高并发访问。
+ 分布式存储
    + MongoDB采用分布式存储架构，数据可以分布在多个服务器上，提供了高可用性和容错性。它使用副本集（Replica Set）和分片（Sharding）技术来实现数据的冗余备份和负载均衡。
+ 强大的查询语言
    + MongoDB提供了丰富的查询功能，包括查询嵌套文档、范围查询、聚合管道等。它还支持全文搜索和地理空间查询，以满足各种数据检索需求。
+ 灵活的数据模型
    + MongoDB的文档模型非常灵活，可以根据需要随时调整数据结构。这使得在应用程序的迭代过程中，数据模型的变更和演进变得更加容易。
+ 数据复制和故障恢复
    + MongoDB的副本集技术提供了数据的冗余备份和故障恢复机制。它使用主从复制来实现数据的持久性和高可用性，当主节点发生故障时，系统可以自动进行切换。

## RABC

### 参考文档
[Mysql版简易示例](RBAC.md)

### 基本介绍

RABC（Role-Based Access Control）是一种基于角色的访问控制模型，用于管理和控制用户对系统资源的访问权限。
在RABC模型中，权限的分配是基于用户所扮演的角色，而不是直接与个体用户相关联。

+ 角色（Role）
    + 角色是一组相关权限和责任的集合，代表着用户在系统中的职能或身份。用户可以被分配一个或多个角色，而不需要为每个用户单独定义和管理权限。
+ 权限（Permission）
    + 权限是指用户在系统中执行某些操作或访问特定资源的权利。每个角色都与一组权限相关联，描述了该角色可以执行的操作和访问的资源。
+ 用户（User）
    + 用户是系统中的个体实体，可以被分配一个或多个角色。通过分配角色，系统可以控制用户对资源的访问权限。
+ 授权（Authorization）
    + 授权是指将角色与权限进行关联和分配的过程。管理员根据用户的职能或身份，将适当的角色授予用户，从而赋予其相应的权限。
+ 认证（Authentication）
    + 认证是确认用户身份的过程，通常涉及用户名和密码、令牌等验证方法。认证和授权是安全访问控制的两个关键环节。
+ 继承（Inheritance）
    + RABC模型支持角色之间的继承关系。这意味着一个角色可以继承另一个角色的权限，简化了权限管理和维护的复杂性。
+ 审计（Audit）
    + 审计是对系统中用户活动和访问操作的记录和监控。通过审计功能，管理员可以跟踪和检查用户的操作行为，以保证系统的安全性和合规性。


<!-- links -->
[your-project-path]:shaojintian/Best_README_template
[contributors-shield]: https://img.shields.io/github/contributors/worst001/note_db.svg?style=flat-square
[contributors-url]: https://github.com/worst001/note_db/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/worst001/note_db.svg?style=flat-square
[forks-url]: https://github.com/worst001/note_db/network/members
[stars-shield]: https://img.shields.io/github/stars/worst001/note_db.svg?style=social
[stars-url]: https://github.com/worst001/note_db/stargazers
[issues-shield]: https://img.shields.io/github/issues/worst001/note_db.svg?style=flat-square
[issues-url]: https://img.shields.io/github/issues/worst001/note_db.svg
[license-shield]: https://img.shields.io/github/license/worst001/note_db.svg?style=flat-square
[license-url]: https://github.com/worst001/note_db/blob/main/LICENSE.txt
