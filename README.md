# 项目简介
本固件适配斐讯 N1 旁路由模式，追求精简纯净!<br>
1、使用LEAN的openwrt源码，目前集成的都是自己需要的一些插件，L大固件默认勾选的部分插件做了精简！<br>
2、自编译脚本吸取各个大佬的精华，重点解决了action编译硬盘不够导致编译失败。（踩过很多的坑，让后来者不要再走弯路）<br>
3、配置文件很精简，自己要什么不要什么增减就行。N1编译必须的Basic Dependence不要精简！<br>
4、目前的配置第一次编译大概是2.5小时左右，第二次编译使用缓存可以节省个把小时。<br>
5、ipv6完整支持！<br>
6、为了拥有自己的定制固件，不停修改测试等待了N多个的编译周期，如果对你有帮助，欢迎fork！<br>
7、集成晶晨宝盒，可以直接在线升级openwrt版本。默认配置的是我的项目地址！<br>
8、内核我测试用的5.15.148很稳定，不建议升级。有部分用户反馈5.15.160以上的内核科学有问题！<br>
# 包含的插件目录如下:<br>
### luci <br>
CONFIG_PACKAGE_luci-app-amlogic=y
CONFIG_PACKAGE_luci-app-dockerman=y
CONFIG_PACKAGE_luci-app-passwall=y
CONFIG_PACKAGE_luci-app-samba4=y
CONFIG_PACKAGE_luci-app-vlmcsd=y
CONFIG_PACKAGE_luci-app-lucky=n
CONFIG_PACKAGE_luci-app-ddns-go=n
CONFIG_PACKAGE_luci-app-uhttpd=y
CONFIG_PACKAGE_luci-app-frpc=n
CONFIG_PACKAGE_luci-app-socat=y
CONFIG_PACKAGE_luci-app-cifs-mount=y
CONFIG_PACKAGE_luci-app-wol=y
CONFIG_PACKAGE_luci-app-mosdns=y
CONFIG_PACKAGE_luci-app-ttyd=y
CONFIG_PACKAGE_luci-app-sqm=y
CONFIG_PACKAGE_luci-app-adguardhome=y
CONFIG_PACKAGE_luci-app-openclash=y

### theme主题<br>
CONFIG_PACKAGE_luci-theme-design=y
CONFIG_PACKAGE_luci-app-design-config=y
CONFIG_PACKAGE_luci-theme-netgear=y
CONFIG_PACKAGE_luci-theme-argon=y
CONFIG_PACKAGE_luci-app-argon-config=y
### vpn插件<br>
CONFIG_PACKAGE_luci-app-openvpn-server=n
CONFIG_PACKAGE_luci-app-softethervpn=n
CONFIG_PACKAGE_luci-app-wireguard=n
CONFIG_PACKAGE_luci-app-zerotier=y
![360截图20241105215446408](https://github.com/user-attachments/assets/5b6381d2-52d7-41d2-af12-a7ea0a6d2598)
![360截图20241105215513569](https://github.com/user-attachments/assets/36f9febd-51bb-41d8-b119-9f9c78967e0a)

***
# 致谢
代码使用LEAN大的[项目](https://github.com/coolsnowwolf/lede)<br>
使用 flippy 的[脚本](https://github.com/unifreq/openwrt_packit)和 breakings 维护的[内核](https://github.com/breakings/OpenWrt/releases/tag/kernel_stable)打包成完整固件，感谢开发者们的无私分享。<br>
flippy 固件的更多细节参考[恩山论坛帖子](https://www.right.com.cn/forum/thread-4076037-1-1.html)。
