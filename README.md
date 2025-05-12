# iOS证书检测介绍
当前版本较上一款ios证书检测源码做出全新升级，功能改进优化。如需了解上一版本查看链接：https://github.com/Forever18/p12certcheck  


##  一、功能如下：  
1.支持在线ios证书检测  
2.自动匹配最新版证书G2、G3、G4、G5协议  
3.支持IPA包证书检测，省去传输ipa过程，用户体验更好  
4.优化检测证书准确性  
5.支持多种证书状态并高亮显示  
6.支持证书掉签时间显示  
7.自动识别证书类型in-house或ad-hoc
8.增加显示证书sha1指纹
9.支持适配任意客户端手机、pc、ipad等设备


## 二、使用方法：
1.首先搭建web服务器  
2.获取证书检测源码  
3.配置web配置文件  

例：  
这里以nginx服务器为例：  

server {  
  listen 80;  
  server_name www.example.com;  
  root /opt/p12certcheck;  

  location / {  
	index  index.html index.htm index.php;  
    }  
}   
说明：  
server_name 这个字段域名根据自已实际情况填写.  
root 这里填写网站源码根路径。  

访问链接：  
http://www.example.com;  

## 三、效果展示：  
![](https://github.com/Forever18/ioscertcheck/blob/main/example/p12.png)  
![](https://github.com/Forever18/ioscertcheck/blob/main/example/ipa.png)  
![](https://github.com/Forever18/ioscertcheck/blob/main/example/provision.png) 

