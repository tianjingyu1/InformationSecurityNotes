1. 连接到数据库服务器
mysql -h host -u root -p xxxx

2. 查看所有库
show databases;

3. 选库
use 库名

4. 查看库下面的表
show tables;

5. 建表
create table msg(
    id int auto_increment primary key,
    content varchar(200),
    pubtime int
) charset utf-8;

6. 添加数据
insert into msg (id,content,pubtime) values (1,'hkjhk',12345)

7. 告诉服务器你的字符集
set names gbk/utf8/...;

8. 查询所有数据
select * from msg;

9. 按id查询一行
select * from msg where id=2/1/....

10. 快速清空表
truncate 表名