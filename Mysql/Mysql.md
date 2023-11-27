# Mysql整理

## 初始密码录入

https://cloud.tencent.com/developer/article/1188636

## 搜索引擎

[引擎比较](https://blog.csdn.net/qq_35642036/article/details/82820178)

1. InnoDB

+ 每条语句默认是一个事务
    + 所以性能没有MyISAM高
+ 聚集索引
    + 所以主键索引的大小会影响副索引
+ 支持外键

2. MyISAM

+ 只有表锁
    + 所以崩溃后无法回复
    + 换来的是批量操作的速度
+ 离散索引
    + 不影响副索引
+ 支持全文索引
    + 只是读的话比InnoDB要快

## 映射表
| MySQL     | JDBCType    | JavaType             | 备注                     |
|-----------|-------------|----------------------|--------------------------|
| char      | CHAR        | String               | 定长字符                 |
| varchar   | VARCHAR     | String               | 变长字符串               |
| tinyint   | TINYINT     | byte                 | 1字节                    |
| smallint  | SMALLINT    | short                | 2字节                    |
| int       | INTEGER     | int                  | 4字节                    |
| float     | FLOAT       | float                | 4字节                    |
| decimal   | DECIMAL     | java.math.BigDecimal | ?字节                    |
| bigint    | BIGINT      | long                 | 8字节                    |
| double    | DOUBLE      | double               | 8字节                    |
| bit       | BOOLEAN     | boolean              | 布尔类型                 |
| date      | Date        | util.Date、sql.Date  | YYYY-MM-DD               |
| time      | TIME        | util.Date、sql.Date  | HH:MM:SS                 |
| timestamp | TIMESTAMP   | util.Date、sql.Date  | YYYY-MM-DD HH:MM:SS      |
| text      | VARCHAR     | String               | 文本类型【2^16-1字节】   |
| longtext  | LONGVARCHAR | String               | 长文本类型【2^32-1字节】 |

## 命令
```bash
/usr/bin/mysql --verbose --help | grep -A 1 'Default options'
```

## 游标与PSCache
[游标](https://www.yiibai.com/mysql/cursor.html)
[PSCache](https://blog.csdn.net/xieyuooo/article/details/99877168)

## 设置root密码

### Mysql 8.0
```bash
# 无密码时登录
./mysql -u root --skip-password

# 查询前，必须要修改密码，如新密码123456:
ALTER USER 'root'@'localhost' IDENTIFIED with mysql_native_password BY '你的新密码';
#刷新权限
flush privileges;
# 首次改密推荐使用本地密码插件 mysql_native_password

use mysql;
select user,host,plugin,authentication_string from user;

# 创建用户任意远程访问
CREATE user 'root'@'%';
# 修改密码
alter user 'root'@'%' identified with mysql_native_password by '123456';
 #给用户授权
grant all privileges on *.* to "root"@"%";
#刷新权限
flush privileges;

# 2. 更改具体用户远程访问
# 创建'root'@'127.0.0.1'用户
CREATE USER 'root'@'127.0.0.1' IDENTIFIED with mysql_native_password BY '123456'; 
#===> 记住刷新权限
flush privileges; 

select user,host,plugin,authentication_string from user;
 
===============5.7以后===================
update user set authentication_string=password("test") where user='root';
update mysql.user set host='你要指定的主机ip' where user='root';

============以下5.7以前======================
SET PASSWORD = PASSWORD('123456');
ALTER USER 'root'@'localhost' PASSWORD EXPIRE NEVER;
flush privileges;
select user,host,plugin,authentication_string from user;
============================================

# 退出mysql>
quit;或者exit;

#关闭mysql
shutdown;

# 修改MySQL用户密码
mysqladmin -u用户名 -p旧密码 password 新密码
 
# 或进入mysql命令行
SET PASSWORD FOR '用户名'@'主机' = PASSWORD(‘密码');
```


