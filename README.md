#####  源码简介：   
本程序用于挂机HostLoc论坛小号刷积分用，方便查看小号积分、等级、金钱等信息。     

#####  系统图片：    
![hostloc_admin.jpg](https://raw.githubusercontent.com/gacjie/hostloc_admin/main/hostloc_admin.png)    

##### 功能说明:    
【账号管理】可自动获取账号信息，挂机时积分、金钱、等级可以手动自动更新。    
【账号开关】账号挂机时登陆错误，会自动关闭该账号状态，状态为off时，则不会执行挂机任务。    
【设置官网】可自定义官网链接，避免官方在主域名与www子域名之间切换。     
【虚拟地址】生成虚拟IP协议头发送给论坛     
【浏览器UA】对账号指定浏览器UA发送给论坛      
【整点执行】设置每日几点开始执行，默认凌晨6点。     
   
##### 项目地址：    
https://github.com/gacjie/hostloc_admin   
https://gitee.com/gacjie/hostloc_admin    
   
##### 更新说明：2024/4/19     
代码整体重构版本    
减少部分功能设置      

##### 安装说明：    
1.设置thinkphp伪静态。     
2.设置public为运行目录，并取消防跨站。   
3.修改runtime文件夹权限777    
4.访问http://域名/install.php安装    
安装完成后可删除以下文件。    
public/database.sql    
public/install.php    
未使用apache可删除以下文件    
public/.htaccess    

##### 手动升级：     
本次为重构版本，请全新安装，重新部署。    

##### 监控任务：     
本次更新URL监控任务改为更为php命令行执行。    
php /您的网站绝对目录/think task     
例如 php /www/wwwroot/hostloc.com/think task      
注意：每次执行计划任务，只对一个账号进行访问空间刷分操作，因此请根据你的账号数设置合理执行的时间。      
