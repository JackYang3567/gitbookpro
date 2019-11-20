# 配置
## 1、创建配置文件book.json
> 进入gitbook_tutorial目录，创建一个文件 book.json  

```
$ npx -p touch nodetouch book.json
```
## 2、编辑配置文件book.json
> book.json文件主要用来存放配置信息，内容如下:  


```
{
    "title": "GitBook简明教程",
    "author": "JackYang",
    "description": "GitBook的安装，gitbook-editor的安装及简单使用",
    "language": "zh-hans",
    "gitbook": "3.2.3",
    "styles": {
        "website": "./styles/website.css",
        "ebook": "./styles/ebook.css",
        "pdf": "./styles/pdf.css",
        "mobi": "./styles/mobi.css",
        "epub": "./styles/epub.css"
   },
    "structure": {
        "readme": "README.md"
    },
    "links": {
        "sidebar": {
            "GitBook简明教程": "https://legacy.gitbook.com/book/jackyangg/"
        }
    },
    "plugins": [
        "-sharing",
        "splitter",
        "expandable-chapters-small",
        "anchors",
        "github",
        "github-buttons",
        "donate",
        "sharing-plus",
        "anchor-navigation-ex",
        "favicon",
        "code"
    ],
    "pluginsConfig": {
       "code": {
            "copyButtons": false
          },
        "github": {
            "url": "https://github.com/JackYang3567"
        },
        "github-buttons": {
            "buttons": [{
                "user": "JackYang",
                "repo": "glory",
                "type": "star",
                "size": "small",
                "count": true
                }
            ]
        },
        "donate": {
              
                    "wechat": "./src/img/微信打赏二维码.jpg",
                    "alipay": "./src/img/支付宝打赏二维码.jpg",
                    "title": "",
                    "button": "赞赏",
                    "alipayText": "支付宝打赏",
                    "wechatText": "微信打赏" 
           },
        "sharing": {
            "douban": false,
            "facebook": false,
            "google": false,
            "hatenaBookmark": false,
            "instapaper": false,
            "line": false,
            "linkedin": false,
            "messenger": false,
            "pocket": false,
            "qq": false,
            "qzone": false,
            "stumbleupon": false,
            "twitter": false,
            "viber": false,
            "vk": false,
            "weibo": false,
            "whatsapp": false,
            "all": [
                "google", "facebook", "weibo", "twitter",
                "qq", "qzone", "linkedin", "pocket"
            ]
        },
        "anchor-navigation-ex": {
            "showLevel": false
        },
        "favicon":{
            "shortcut": "./src/img/favicon.jpg",
            "bookmark": "./src/img/favicon.jpg",
            "appleTouch": "./src/img/apple-touch-icon.jpg",
            "appleTouchMore": {
                "120x120": "./src/img/apple-touch-icon.jpg",
                "180x180": "./src/img/apple-touch-icon.jpg"
            }
        }
    } 
}
```

## 3、配置文件book.json中各属性介绍

 * #### 1、title 本书标题
 * #### 2、author 本书作者
 * #### 3、description  本书描述
 * #### 4、language  本书语言，中文设置 "zh-hans" 即可

 language” : “zh-hans”  
 
 可选的语言如下：
```
 en, ar, bn, cs, de, en, es, fa, fi, fr, he, it, ja, 
 ko, no, pl, pt, ro, ru, sv, uk, vi, zh-hans, zh-tw
 ```
 * #### 5、gitbook  指定使用的 GitBook 版本
 * #### 6、styles  自定义页面样式

 默认情况下各generator对应的css文件
```
    "styles": {
        "website": "styles/website.css",
        "ebook": "styles/ebook.css",
        "pdf": "styles/pdf.css",
        "mobi": "styles/mobi.css",
        "epub": "styles/epub.css"
    }
```
 * #### 7、structure  指定 Readme、Summary、Glossary 和 Languages 对应的文件名
 * #### 8、links  在左侧导航栏添加链接信息
 ```
 "links": {
        "sidebar": {
            "GitBook简明教程": "https://legacy.gitbook.com/book/jackyangg/"
        }
    },
 ```
 * #### 9、plugins  配置使用的插件
 可以在插件前面加-符号删除默认插件，默认五种插件如下，更多插件

  - highlight：代码高亮
  - search：导航栏查询功能（不支持中文）
  - sharing：右上角分享功能
  - font-settings：字体设置（最上方的"A"符号）
  - livereload：为GitBook实时重新加载

 * #### 10、pluginsConfig  配置插件的属性