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
