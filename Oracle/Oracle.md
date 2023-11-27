# Oracle

## 数据类型的坑
数据类型是浮点数 小数是0
在使用 Mybatis 时 Dto 必须为浮点 BigDemical
否则会不报错但查询的结果只有一条记录

## 类型映射
 | Oracle SQL 型（8i 版）   | JDBC 数据类型   | Java 数据类型          |
 | ------------------------ | --------------- | ---------------------- |
 | NUMBER                   | BIT             | boolean                |
 | NUMBER                   | TINYINT         | byte                   |
 | NUMBER                   | SMALLINT        | short                  |
 | NUMBER                   | INTEGER         | int                    |
 | NUMBER                   | BIGINT          | long                   |
 | NUMBER                   | FLOAT           | double                 |
 | NUMBER                   | REAL            | float                  |
 | NUMBER                   | DOUBLE          | double                 |
 | NUMBER                   | NUMERIC         | java.math.BigDecimal   |
 | NUMBER                   | DECIMAL         | java.math.BigDecimal   |
 | CHAR                     | CHAR            | String                 |
 | VARCHAR2                 | VARCHAR         | String                 |
 | LONG                     | LONGVARCHAR     | String                 |
 | DATE                     | DATE            | java.sql.Date          |
 | DATE                     | TIME            | java.sql.Time          |
 | DATE                     | TIMESTAMP       | java.sql.Timestamp     |
 | NUMBER                   | BINARY          | byte[]                 |
 | RAW                      | VARBINARY       | byte[]                 |
 | LONGRAW                  | LONGVARBINARY   | byte[]                 |
 | BLOB                     | BLOB            | java.sql.Blob          |
 | CLOB                     | CLOB            | java.sql.Clob          |
