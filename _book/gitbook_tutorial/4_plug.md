# 插件
## 1、GitBook 插件列表
* ### back-to-top-button（返回顶部）
* ### code（代码添加行号&复制按钮）
* ### search-pro（高级搜索，支持中文）
* ### github（在右上角添加github图标）
* ### splitter（侧边栏宽度可调节）
* ### tbfed-pagefooter（页面添加页脚，简单的）
* ### page-copyright（页面页脚版权，复杂的）
* ### donate（打赏插件）
* ### sharing-plus（分享当前页面）
* ### custom-favicon（修改标题栏图标）
* ### prism（代码高亮）
* ### todo（复选框）
* ### pageview-count（阅读量计数）
* ### auto-scroll-table（表格滚动条）
* ### image-captions（显示图片名称）
* ### styles-sass（使用sass替换css）
* ### styles-less（使用less替换css）
* ### toggle-chapters（目录折叠）
* ### multipart（分章节展示）
* ### 设置导航序号

## 2、添加插件
在book.json中配置如下（这里用code插件作为例子）： 

```
{
    "plugins": [
        "code"
    ],
    "pluginsConfig": {
        "code": {
            "copyButtons": false
        }
    }
}
```

## 3、安装插件
可以选择下列三种方式中的一种进行安装  
 - ### 1）、执行gitbook install
  这其实是安装book.json中的配置
  ```
    $ gitbook install ./
  ```  
 - ### 2）、npm安装
 命令格式npm install gitbook-plugin-插件名字
 ```
 $ npm install gitbook-plugin-code
 ```
 - ### 3)、从GitHub下载源码，放到node_modules文件夹里
