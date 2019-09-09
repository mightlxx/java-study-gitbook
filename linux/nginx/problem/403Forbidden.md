# 403 Forbidden

nginx 访问静态资源文件提示

![image-20190908163131411](./img/image-20190908163131411.png)

是因为权限引起，将nginx 改成root启动

```
 #user nobody;
 user root;
```

