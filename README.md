# window+iis8+sqserver2017+django2.0填坑。
各种坑

python3.4，不然多少坑也跳不完。

步骤

1 写个hello  测试hello

2 wfastcgi 安装，复制。

3 iis配置  处理程序映射  fastcgi设置变量 3个参数  回收网站。

4 settings 里面ALLOWED_HOSTS = ['*']

5 One more thing，Python的各种模块，直接打包复制了。或者整个虚拟环境带过来（这个没有试）

6 sql server的步骤

    （1）导出脚本。
  
    （2）导入数据，但是会遇到个坑，需要用安装工具安装一个ssis的东西，就是Integration Services
    
     (3) 执行一下
     
    （4）数据库总安全性，添加登陆角色。设置为 bd_owner 
    
     （5）beauty安全性，设置bd_owner
     
     (6) 检查是否是混合验证模式。
