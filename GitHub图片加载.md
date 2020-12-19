# 解决DNS污染（github图片不加载）

## 解决问题的思路：
图片挂掉了，shift+ctrl++c放到挂到的图片上  
在右侧会显示图片资源的地址，截取主地址。（就是截止到.com那)  
通过`https://www.ipaddress.com/`查询网址的DNS
更新到host文件


SwitchHosts工具  
`下载地址`
https://github.com/oldj/SwitchHosts/releases

**（但是有一个问题，使用下面的dns地址后，原本不能加载的图片可以加载了，但是原本能加载的图片如头像，却挂了）**

140.82.121.4 github.com  
140.82.121.3 gist.github.com  
185.199.108.153 assets-cdn.github.com  
151.101.248.133 raw.githubusercontent.com  
151.101.248.133 gist.githubusercontent.com  
151.101.208.133 cloud.githubusercontent.com  
151.101.208.133 camo.githubusercontent.com  
151.101.208.133 avatars0.githubusercontent.com  
151.101.248.133 avatars1.githubusercontent.com  
151.101.208.133 avatars2.githubusercontent.com  
151.101.248.133 avatars3.githubusercontent.com  
151.101.208.133 avatars4.githubusercontent.com  
151.101.248.133 avatars5.githubusercontent.com  
151.101.208.133 avatars6.githubusercontent.com  
151.101.208.133 avatars7.githubusercontent.com  
151.101.208.133 avatars8.githubusercontent.com  
185.199.111.154 github.githubassets.com  
140.82.121.5 api.github.com  

# 2020-12-19更新

**参考：** https://github.com/itgoyo/500Days-Of-Github/issues/231

但是完全使用上述dns后，github明显变慢，而且头像加载不出来了？

**实测可行：**

140.82.114.4 github.com  
140.82.114.3 gist.github.com  
185.199.108.153 assets-cdn.github.com  
151.101.64.133 raw.githubusercontent.com  
151.101.108.133 gist.githubusercontent.com  
151.101.108.133 cloud.githubusercontent.com  
151.101.108.133 camo.githubusercontent.com  
151.101.108.133 avatars0.githubusercontent.com  
151.101.108.133 avatars1.githubusercontent.com  
151.101.108.133 avatars2.githubusercontent.com  
151.101.108.133 avatars3.githubusercontent.com  
151.101.108.133 avatars4.githubusercontent.com  
151.101.108.133 avatars5.githubusercontent.com   
151.101.108.133 avatars6.githubusercontent.com  
151.101.108.133 avatars7.githubusercontent.com  
151.101.108.133 avatars8.githubusercontent.com  

# 图床
**视频链接教学：** https://www.bilibili.com/video/BV1Lt411J7Mp?from=search&seid=13082337418571714831  
**所用软件及地址：** **Picgo** https://github.com/Molunerfinn/PicGo
 
