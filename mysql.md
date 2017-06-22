# 数据库
### 更新源
*用vim打开源列表*
sudo vim /etc/apt/sources.list

*将里面的源粘贴到源列表里*

## Apache安装

1. sudo apt-get update
2. sudo apt-get install tasksel
3. sudo tasksel

## MySQL命令行操作
连接Mysql 格式： mysql -h 主机地址 -u用户名 －p用户密码

### 支持中文
建表的时候就要使用utf8编码
```sql 
create table entries2 (
        id     int auto_increment, 
        title  text,
        content  text,
        posted_on  datetime,
        primary key (id)   
) character set = utf8;
```
#### 创建数据库
  create database <数据库名>
#### 显示数据库
  show databases 
#### 删除数据库
  drop database <数据库名>
#### 使用数据库
   use <数据库名>
   
##### 创建数据表
 命令：create table <表名> ( <字段名1> <类型1> [,..<字段名n> <类型n>]);
##### 查看表结构
 desc 表名
##### 删除表
 命令：drop table <表名>
##### 表插入数据
 命令：insert into <表名> [( <字段名1>[,..<字段名n > ])] values ( 值1 )[, ( 值n )]
##### 查询表中的数据
1. 查询所有行 命令： select <字段1，字段2，...> from < 表名 > where < 表达式 >
2. 查询前几行数据 例如：查看表 MyClass 中前2行数据 mysql> select * from MyClass order by id limit 0,2;
select一般配合where使用，以查询更精确更复杂的数据
##### 修改表中的数据
 语法：update 表名 set 字段=新值,... where 条件
 
