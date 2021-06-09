# LDBMS —— A simple DBMS

## 1.0 实现创建用户功能
## 2.0 实现数据库的创建和删除
    create database 数据库名;
    drop database 数据库名;
## 3.0 实现数据表的创建（t为数据表名）与删除
    create table t(name char(int) not null,age int,sex boolean);
    drop table 数据表名;
## 4.0 实现向数据表中插入数据
    insert into t(name,age,sex) values("mary",18,0);
    insert into t(name,age,sex) values("Tom",19,1);
## 5.0 删除数据表中的元素
    delete from t where age="mary";
## 6.0 更新表中的数据
    update t set age=20 where name="Tom";
## 7.0 查询数据表中的数据
    select * from t;                            //数据表t的所有数据
    select * from t where age=18;               //查询数据表t中age=18的所有数据
    select age,sex from t where name="Tom";     //查询数据表t中name="Tom"的age和sex信息
## 8.0 使用数据库
    use 数据库名;
## 9.0 显示当前数据库中的数据表或显示当前用户的数据库
    display tables;       //显示当前使用的数据库下的所有数据表
    display databases;    //显示当前用户下的所有数据库
