
1. aop  面向切面编程

aspectJ 项目,  spring aop


2. spring中的aop

基本概念:

目标: 
切点: 在哪里切, pointcut
切面: 点加起来就成面
通知: 在切点上做什么事情  advisor

用切点找到目标,在它身上执行通知操作

3. helloworld
切点表达式
execution(   *  com.etc.UserService.*  (..)                   )                                     )
          返回值                               所有方法  任意参数

execution(* com..*(..))
                     包以及子包

spring如何实现aop的
1).动态代理 jdk
2) 织入  去分析.class文件,去修改class将代码插入
   cglib

4. 通知 
五种通知 

前置
后置
前后(环绕)
返回值, 不能改结果
异常, 只有代码出现异常的才会进入

5. spring+jdbc
数据源

连接池 
tomcat
druid
dbcp 
c3p0
