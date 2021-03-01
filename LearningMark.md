## naco源码 服务本地安装步骤

step1:

从github上，下载nacos最新的源码到本地:

git clone https://github.com/alibaba/nacos.git

step2:

本地编译(建议用阿里云的maven仓库):

mvn -Prelease-nacos -Dmaven.test.skip=true clean install -U

step3:

源码运行时，通常使用的是单机模式，因此需要在启动参数中进行设置，在jvm的启动参数中，添加

-Dnacos.standalone=true

step4:

编译完成的nacos源码导入到idea开发工具中；进入到nacos-console模块下，启动该模块下的com.alibaba.nacos.Nacos类

启动成功，请享用。

http://localhost:8848/nacos/index.html

登录名/密码 nacos/nacos
