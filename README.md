### 
- 基于 chongshengB 项目修改。
- 完全精简了插件和系统组件，只保留了ssh、smartdns、frp、zerotier。其中smartdns更新到官网最新版，即2020/9/8的3.3版本。
- B大 smartdns.sh脚本有bug。web控制台smartdns界面“禁用IPV6解析”选项，点击打开或关闭均无效，原因是sh文件里snds_ipv6和sdns_ipv6搞反了，所以自己修改了变量名称和判断逻辑。随便增加了以下参数
   - 修改“禁用IPV6解析”变量名和判断逻辑
   - 持久化缓存cache-persist yes 
   - 缓存持久化文件路径cache-file /tmp/smartdns.cache
   - web控制台输入的ttl、ttl_min、ttl_max值，写入到smartdns.conf配置文件中
   - log-level warn 
   - 日志文件路径/tmp/smartdns.log

### 固件说明 ###
* 默认登陆IP:192.168.2.1 
* 默认用户名/密码:admin/admin
* 默认wifi密码:1234567890


### 请参阅 ###
- https://www.jianshu.com/p/cb51fb0fb2ac
- https://www.jianshu.com/p/6b8403cdea46

### 特别说明 ###
* hanwckf源码：https://github.com/hanwckf/rt-n56u
* lean源码: https://github.com/coolsnowwolf/lede
* 汉化字典来自：https://github.com/gorden5566/padavan
* hanwckf更新日志：https://www.jianshu.com/p/d76a63a12eae

