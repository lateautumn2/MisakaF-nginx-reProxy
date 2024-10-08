# MisakaF-nginx-reverse-proxy

这是关于MisakaF Emby 公费服/机场服的反代基础配置

如果您认为该配置有误，欢迎提交PR，thanks


```
# debian
cd /etc/nginx/conf.d/
nano misakaf.conf

#将配置文件内容粘贴进去，并修改对应的example域名，保存并退出

nginx -t
systemctl reload nginx
```

