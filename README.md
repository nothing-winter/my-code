# my-code

## git 使用svn 仓库

git svn clone svn://127.0.0.1/xxx/xxx --username=xxx

git config --global core.autocrlf true 

Git可以在你提交时自动地把行结束符CRLF转换成LF，而在签出代码时把LF转换成CRLF。用core.autocrlf来打开此项功能，如果是在Windows系统上，把它设置成true，这样当签出代码时，LF会被转换成CRLF:



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

# Spring BeanPostProcessor加载顺序
BeanPostProcessor 分为三层 
*   第一层为实现org.springframework.core.PriorityOrdered接口
*   第二层为实现org.springframework.core.Ordered接口
*   第三层为余下的BeanPostProcessor  

只有同层的BeanPostProcessor创建完了才会进行Processor注册       
当BeanPostProcessor引用了普通Bean，将在创建BeanPostProcessor时创建普通Bean
加载顺序源码org.springframework.context.support.PostProcessorRegistrationDelegate#registerBeanPostProcessors(
			ConfigurableListableBeanFactory beanFactory, AbstractApplicationContext applicationContext)

#awk
在windows下使用 && 需要转义 ^&^&
			
