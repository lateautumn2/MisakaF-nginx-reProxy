# Emby播放分离反代示例

1、Misakaf.conf

这是关于MisakaF Emby 公费服/机场服的反代基础配置
（补充：pilipili的结构与misakaf一致）

```
# debian
cd /etc/nginx/conf.d/
nano misakaf.conf

#将配置文件内容粘贴进去，并修改对应的`#注释`区域，保存并退出

nginx -t
systemctl reload nginx
```
2、embyplus.conf

这是关于embyplus（纸片人） Emby 公益服的反代基础配置
- 由于目前纸片人有单独的推流线路，所以需要2次重定向
- 你在纸片人bot中选的每一条线路相对的推流域名都不同，但仅仅是线路推流域名不同（即第二次重定向），默认推流域名（即第一次重定向）是不变的
- 建议在纸片人bot中选择默认线路，cf线路不论你使用那个区域的反代vps都能获得相对较好的体验

```
# debian
cd /etc/nginx/conf.d/
nano embyplus.conf

#将配置文件内容粘贴进去，并修改对应的`#注释`区域，保存并退出

nginx -t
systemctl reload nginx
```
