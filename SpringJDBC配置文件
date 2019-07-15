<!-- 配置数据源-->
    <bean id="dataSource" class="com.alibaba.druid.pool.DruidDataSource">
        <!-- Mysql数据库驱动-->
        <property name="driverClassName" value="com.mysql.jdbc.Driver"></property>
        <!-- 连接数据库的url-->
        <property name="url" value="jdbc:mysql://localhost:3306/test?characterEncoding=utf8"></property>
        <!-- 连接数据库的用户名-->
        <property name="username" value="root"></property>
        <!-- 连接数据库的密码-->
        <property name="password" value=""></property>
    </bean>

    <!-- 配置Jdbc模板-->
    <bean id="jdbcTemplate" class="org.springframework.jdbc.core.JdbcTemplate">
        <property name="dataSource" ref="dataSource"></property>
    </bean>

    <bean id="userDAO" class="com.etc.dao.UserDAO">
        <property name="jdbcTemplate" ref="jdbcTemplate"></property>
    </bean>
