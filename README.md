# jws-demo
test JAX_WS
############################################################
搭建sonatype nexus环境，将jws-common相比打包证Jar上传
到sonatype，jws-client依赖于jws-common项目;
<dependency>
	<groupId>org.donald</groupId>
	<artifactId>jws-common</artifactId>
	<version>${jws.demo.version}</version>
</dependency>
上面这种方式为静态引入公共基础包；也可以动态引入公共基础包，在build path中
添加项目引用，同时添加上述的jws-common依赖，建议使用第二种方式，当公共基础包
变更时，及时发现。
#############################################################
jws-demo下面有三个模块,用于测试JAX-WS：
jws-server：WebService服务端
jws-client：客户端
jws-common：工具包
##############################################################
此项目为Jws_client与Jws_Server的集成，并抽出共同的工具类到jws-common项目。

