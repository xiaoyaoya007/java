<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:context="http://www.springframework.org/schema/context"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd
       http://www.springframework.org/schema/context
        http://www.springframework.org/schema/context/spring-context.xsd "
        >

    <!--set方法注入  value/ref -->
    <bean id="user" class="com.etc.User">
        <property name="name" value="xiaoming"></property>
    </bean>
    
    <!--构造方法注入  value/ref -->
    <!--
    <bean id="student" class="com.etc.Student">
        <constructor-arg type="java.lang.String" name="name" value="aaa"></constructor-arg>
    </bean>
    -->

    <!--component注解方式（类前面要加一个@Component，以及导包）告知Spring在创建容器时要扫描的包-->
    <context:component-scan base-package="com.etc"> </context:component-scan>
    
</beans>
