#docker项目运行结构

work-compose<br>
以下路径请注意查看<br>

certs #证书文件路径<br>

linux #linux系统下的docker-compose.yml    
 
logs  #日记目录

    -mysql
    -nginx
    -php
    -php-fpm
    
mongo #mongo目录

    -config
    -db
    
mysql5.7 #mysql目录

    -data
    -my.cnf
    
nginx1.17.4 #nginx目录

    -conf.d #网站的nginx
        -default.conf #默认网站
    -nginx.conf
    
php7.2.18   #php目录

    -ext  #php扩展件
    -fpm  
    -php.ini    #php配置信息
    
php7.2.18-fpm  #php目录

    Dockerfile  #php运行的环境需求
    
redis5.0.6     #redis

    -data
    -redis.conf
    
windows  #linux系统下的docker-compose.yml     
-www	#网站运行的目录，所网站都需要经过这个目录

<h3>请注意：</h3>
<h3>
1.如你的环境使用linux，请把linux目录内的docker-compose.yml
拿到../目录
</h3>
<h3>
2.如你的环境使用windows，请把windows目录内的docker-compose.yml
  拿到../目录
</h3>


更多技术请关注
 
 微信公众号：技术共享社区
 
 <img src="https://raw.githubusercontent.com/hwkkevin/wechat_qrcode/master/images/qrcode.jpg" width="300" height="300"/>
 
 今日头条：技术共享社区
 
 <img src="https://raw.githubusercontent.com/hwkkevin/wechat_qrcode/master/images/headlines.jpeg" width="300" height="300"/>
 
 百家号：技术共享社区
 
 网站访问：https://baijiahao.baidu.com/u?app_id=1621784986732890
 
 个人博客：技术共享社区
 
 域名：https://www.jzgblog.com
 
 支持我的技术的，请打赏一个谢谢。
 
 微信打赏
 
 <img src="https://raw.githubusercontent.com/hwkkevin/wechat_qrcode/master/images/wechatpay.jpg" width="300" height="450"/>
 
 支付宝打赏
 
 <img src="https://raw.githubusercontent.com/hwkkevin/wechat_qrcode/master/images/alipay.jpg" width="300" height="450"/>
 
 
 
 
 





