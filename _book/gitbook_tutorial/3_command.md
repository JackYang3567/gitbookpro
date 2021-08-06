# 命令
GitBook常用的一些命令

## 1、查看gitbook的帮助信息
```
$ gitbook --help
```
## 2、启动服务器生成静态网页预览
```
$ gitbook serve
```
## 3、生成静态网页而不开启服务器
```
$ gitbook build
```
## 4、生成静态网页时指定gitbook的版本，如果本地没有将先下载
```
$ gitbook build --gitbook=3.2.3
```

## 5、列出所有的gitbook版本
```
$ gitbook ls
```
## 6、列出远程可用的gitbook版本
```
$ gitbook ls-remote
```
## 7、更新到gitbook的最新版本
```
$ gitbook update
```
## 8、卸载对应的gitbook版本
```
$ gitbook uninstall 3.2.3
```
## 9、安装依赖
 > 主要指在 book.json 中加入的配置插件  
 
```
$ gitbook install ./
```
## 10、指定log的级别
```
$ gitbook build --log=debug
```
## 11、输出错误信息
```
$ gitbook builid --debug
```