## stu数据库中4个表的结构

information(学生)表：

 属性 | 类型 | 长度 | 说明 
------|------|------|------
 sno | char | char(10) | 主键 
 sname | char | char(10) | 不能为空
 sex | char | char(5) | 不能为空
 age | char | char(5) | 不能为空
 sdept | char | char(10) | 外键

score(成绩)表：

 属性 | 类型 | 长度 | 说明 
 ------|------|------|------
 sno | char | char(10) | 主键
 cno | char | char(5) | 主键
 score | char | char(3) | 取值为0-100
 
 school(学校)表：
 
 属性 | 类型 | 长度 | 说明 
 ------|------|------|------
 sdept | char | char(10) | 主键
 major | char | char(20) | 不能为空
 
 course(课程)表：
 
 属性 | 类型 | 长度 | 说明 
 ------|------|------|------
 cno | char | char(5) | 主键
 cname | char | char(10) | 不能为空
 sdept | char | char(10) | 外键
 
