maven

是apache软件基金会一个项目, 用来管理项目的项目,整个生命周期 
创建一个项目,下载jar包,写代码,编译,测试,打包,发布

自动发布系统,纯命令行的工具 


注意点:
安装后的配置 ,将settings.xml拷贝到 .m2/settings.xml

1.基本概念

仓库 Repository:  jar包
远程仓库: 完整, maven.org
镜像仓库: 远程仓库的镜像 ,  公司内部 

<mirror>
        <id>nexus-aliyun</id>
        <mirrorOf>*</mirrorOf>
        <name>Nexus aliyun</name>
        <url>http://maven.aliyun.com/nexus/content/groups/public</url>
    </mirror>

本地仓库:  曾经用过的jar包
<localRepository>/path/to/local/repo</localRepository>

2. pom
project object model 工程对象模型 
是一xml文件 ,是和项目在一起的, 描述项目的

依赖  dependency
插件
执行等 

3. 生命周期 -跟命令绑定 

开始(新建) -> validate(校验) -> compile(编译) -> test(单元测试) -> package(打包) -> vertify -> install ->        deploy -> 结束 
                                                                                                   war, jar                校验         安装到仓库中  本地发布
mvn validate 
mvn compile


4. 插件 
插件和生命周期绑定在一起的

5. maven命令的使用
1) 创建项目
mvn archetype:generate -DarchetypeArtifactId=maven-archetype-quickstart -DgroupId=com.etc -DartifactId=mavehello 

版本号 snapshot临时版本  release发布版本



a. 安装maven
b.配置  镜像  ,
c. 创建一个项目 
d. 打包项目 



6. idea 中maven的使用


