![分流](https://user-images.githubusercontent.com/73426989/150645780-77bf292a-ecbf-4908-88c0-d57ec44d455b.png)               

passwall按URL地址/网址/IP分流教程图↑                  

* 上图中的建立分流控制节点这一步骤已经不需要你操作了，最新passwall插件已经默认帮你建立好了！
* 只要是passwall支持的协议的线路，都可以按照地址分流规则指定不同的线路

默认的基础分流规则肯定不够你用的，需要自行添加其他的网站的域名等新规则，关于如何新建自己想要的分流规则举例：        
比如采用v2fly的规则举例添加telegram域名分流规则：           

首先访问 [规则文件](https://github.com/v2fly/domain-list-community/tree/master/data)            

![1](https://user-images.githubusercontent.com/73426989/150645906-2e3ba5ef-aa86-4559-aed7-f96325962edd.jpg)           

然后浏览器中 Ctrl+F键 查找你要找的名字 telegram不必打全就可能定位到此条规则了                   

![2](https://user-images.githubusercontent.com/73426989/150645966-4d9d052f-00c5-4a21-b148-9db17e0658f7.jpg)            

进去复制所有域名，粘贴到新建的passwall分流规则里，保存并应用即可完成telegram分流规则的添加              

![3](https://user-images.githubusercontent.com/73426989/150646042-da78e6a1-b7c0-4d85-9c71-e37e3f74913a.jpg)            

![4](https://user-images.githubusercontent.com/73426989/150646063-f5ead300-fa17-4923-b4ae-e2b2cf6c7e27.jpg)          

![5](https://user-images.githubusercontent.com/73426989/150646069-838f35e5-e4e9-4bb3-adb5-8c85699b4085.jpg)           

同理。你可以添加其他的你需要的分流规则。                 
简直不要太简单实用的分流规则添加。             
还有谁不知道passwall可以如此简单建立分流的你就打死他(*^_^*)                     
提醒：最好从不同的知名的维护较为勤的规则里都抄出来你需要的域名及IP形式的规则，组合成你自己的完备的一个分流规则集。仅抄一个不太能保证没有漏掉的域名                    


[返回主页](https://boduoyejieyi666.github.io/whonolikeboduoyejieyi/)                  


