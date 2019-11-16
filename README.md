# my-code
### Linux下Mysql 大小写敏感
### 线上出现Bug 先寻找有没有类似问题,再估计影响范围，寻找解决方法，修复bug

#创建mongodb 用户
db.createUser(
   {
     user: "root",
     pwd: "root",
     roles: [ { role: "userAdminAnyDatabase", db: "admin" } ]
   }
 )


#Java
方法调用的传递
对于基本类型，赋值运算符会直接改变变量的值，原来的值被覆盖掉。  
对于引用类型(Object) ，赋值运算符会改变引用中所保存的地址，原来的地址被覆盖掉。但是原来的对象不会被改变（重要）。  
参数传递基本上就是赋值操作  
引用提供了改变自身方法的引用类型（可以修改对象） 
https://www.zhihu.com/question/31203609

# Mysql 空字符不敏感
当select * from Player where name = "A "时，会获得A
