2020-01-07学习内容
=================
Sphinx,Git,Maven,Spring Boot CLI

Sphinx
----------------
http://fsdtraining.com/en/latest/pages/sphinx.html

列表:

 * Java
 * Spring Boot

自动递增的数字:

 #. Sphinx
 #. Spring Boot CLI

部署到Read the Docs上
--------------------
https://readthedocs.org/projects/my-wiki-mei/

Maven学习
--------------------
mvn生命周期的命令：
 #. mvn clean：清理编译的项目
 #. mvn compile：编译项目
 #. mvn test：测试项目（运行测试类）
 #. mvn package：负责将我们的项目打包
 #. mvn install：将这个项目安装到仓库中

修改密钥的权限：
chmod 700 /home/Memir/.ssh/id_rsa  

Maven使用多线程加速install:(进入有POM文件的Maven工程下面)
 #. mvn -T 4 clean install
 #. mvn -T 1C clean install 

Maven install过程中跳过测试：
 #. mvn -T 4 clean install -DskipTests
 #. mvn -T 4 clean install -Dmaven.test.skip=true 

Nexus
--------------------
搭建Nexus私服的目的：解决工作上组件之间的jar包依赖管理。

使用Aliyun国内镜像
--------------------
::

	<mirrors>
        <mirror>
            <id>alimaven</id>
            <name>aliyun maven</name>
            <url>
                http://maven.aliyun.com/nexus/content/groups/public/
            </url>
            <mirrorOf>central</mirrorOf>
        </mirror>
    </mirrors>


Git
========

RPC
-------
RPC(Remote Procedure Call)远程过程调用，也就是一个节点请求另一个节点提供的服务。