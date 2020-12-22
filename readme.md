# TeambitionShare
挂载Teambition文件 直链分享  
已支持Teambition网盘(需申请)与Teambition项目  
PHP版本推荐 >= 5.6  
伪静态规则分别在.htaccess 和 nginx 文件中  
项目挂载演示站点:[tbfile.ouoacg.com](http://tbfile.ouoacg.com)  
网盘挂载演示站点:[tbfile.ouoacg.com/pan](http://tbfile.ouoacg.com/pan)  
访问密码:123456  
## 一些问题
1.Cookie有效期  
目前我自己的Cookie使用了1个多月未失效,猜测只要你不在官网手动退出登录就不会失效  
2.下载速度(Teambition项目)  
开源前测试能跑到20MB/s,2020-12-17测试时速度下架到1MB/s左右  
2020-12-18 测试能到10MB+/s 然后会下降到1MB/s  
感觉下载速度有点不稳定  
3.访问密码(目前只支持全局密码)  
添加访问密码在config/app.cfg.php中添加 'password' => '你要设置的密码' 即可  
4.二级目录运行  
放在二级目录运行,配置的时候填入对应的URL和修改伪静态规则即可  
## 如何使用
1.1版本未进行配置时会自动跳转配置向导  
先去 www.teambition.com 注册登录  
然后去项目 创建一个项目  
![image](https://ae01.alicdn.com/kf/U78fa30b3f30b47de96af1449808e153cV.jpg)  
然后获取Cookie和项目ID 填到config/app.cfg.php中  
![image](https://ae01.alicdn.com/kf/U6ac816255ae44212a0b10f8d56b8cc01k.jpg)  
![image](https://ae01.alicdn.com/kf/Ube8a1476632a48c59f760d19fec97f79F.jpg)  