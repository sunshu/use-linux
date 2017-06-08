# Kotlin 安装,学习
---
>  内容多数来源于网络， 

## 地址
     [官网地址 : kotlincn.net]( www.kotlincn.net)
     [中文地址 : kotlincn.net](www.kotlincn.net)
     [文档资料 : gitbook](https://huanglizhuo.gitbooks.io/kotlin-in-chinese/content/)
     [掘金:kotlin 资源](https://juejin.im/post/591dd9f544d904006c9fbb96)
	
## 试用
 kotlin 也可以[在线试用 ](https://try.kotlinlang.org/#/Examples/Hello,%20world!/Simplest%20version/Simplest%20version.kt)
    	
### 安装  

 * Intellij IDE ,Android Studio 最新的版本已经集成进去，旧版本在 File -> Settings -> Plugins 中搜索 kotlin 选择安装
     ![](imgs/20170608-123111.png  =100x)
     
* Eclipse 在 Help -> Eclipse Marketplace 中搜索 kotlin 
    ![](imgs/20170608-123513.png =100x)
    
   * 命令行中构建
    	1.  安装sdkman   
    	[sdkman地址](sdkman.io)
	[sdkman github](https://github.com/sdkman/sdkman-cli)
		```  $ curl -s https://get.sdkman.io | bash   ```
		```source "$HOME/.sdkman/bin/sdkman-init.sh" ```
    	2. 通过sdkman 安装kotlin
    	``` sdk install kotlin```
    	3.  sdkman 安装过程中需要root 账号，普通用户执行命令后  ./sdkman/bin/ 目录下没有 sdkman-init.sh 这个脚本，需要删除 ~/.sdkman 下重新下载
    	4. 目前尝试好几次，kotlin 下载应该需要翻墙 ，目前下载一般卡住
    	5. 也尝试其他方式下载 ： 通过    [ubuntu-make] (https://wiki.ubuntu.com/ubuntu-make)    下载也是
    	
    	
	
    	

    	



