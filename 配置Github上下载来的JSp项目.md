# 配置项目备忘录
## 主体思路
* 配置Tomcat服务器
    * 1.右上角添加自己版本的Tomcat服务器（此时还没有给服务器添加运行文件）
    * 2.打开project structure------>Artifacts----->(一般情况是空的)----->  +  ----->Web Applacation Exploded----->From Module  
    **(完成效果图)**
    ![](https://pic.downk.cc/item/5fe734ca3ffa7d37b3ce22f5.png)
    * 3.向Tomcat服务器中添加war包
    Deployment----> + ----->Artifacts(就是添加2.的包)  
    ![](https://pic.downk.cc/item/5fe735c63ffa7d37b3cfb0f7.png)
* 配置jar包
    * 有的时候需要自己如jsp-api或者sevlet-api等包（都是Tomcat的jar下的）
    * 甚至有可能使用第三方包，如fastjson
* 配置数据库文件
    * 一般项目都会自带，添加到navicat就好了 
## 问题解决
* **localhost：1.99端口正在占用**：
    不要傻乎乎的再去重启或者使用命令行查找进程，在tomcat的安装目录的bin下，有一个shutdown.bat文件，关闭在重启一下tomcat就好了