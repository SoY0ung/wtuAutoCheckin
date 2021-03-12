# wtuAutoCheckin
WTU Health Code Auto Check in for iOS (Shortcut App)

**The script is only for iOS 13+, Android version is not available**

启发自 [loyio的wtuHealthCode](https://github.com/loyio/wtuHealthCode)

## 说明
**本打卡脚本仅供学习交流使用，请勿过分依赖。开发者对使用或不使用本脚本造成的问题不负任何责任，不对脚本执行效果做出任何担保，原则上不提供任何形式的技术支持。**

## 使用方法

### 写在前面：

**本脚本需要用到你的个人标识符(Authorization)数据，需要自行抓包获取，如果你连抓包都不知道，就不用再往下看了 ;P**

推荐的抓包软件：[Stream](https://apps.apple.com/cn/app/stream/id1312141691)

配置和抓包过程请看：[抓包实践](https://www.jianshu.com/p/a34585836b3a) 

1. **抓包**

    抓到的包形如这样：
 ```
 Host: jk.wtu.edu.cn
Connection: keep-alive
Content-Length: 726
content-type: application/x-www-form-urlencoded
Authorization: eyJxxxxxxx............xxxxxxxxxxxxg
Accept-Encoding: gzip,compress,br,deflate
User-Agent: Mozilla/5.0 (iPhone; CPU iPhone OS 14_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 MicroMessenger/8.0.2(0x18000234) NetType/WIFI Language/zh_CN
Referer: https://servicewechat.com/wx1sssc7/12/page-frame.html
```   
   记录下它的Authorization(也就是个人标识符)

2.**运行快捷指令**


  打开指令后进行配置，输入你的个人标识符(Authorization)和其他信息(用于生成打卡)，然后运行即可。
  
  
  **提示错误时请检查Authorization是否填对，不建议更改“所在地点”和“返校情况”，不然可能会导致出错**
  
  *建议放在捷径App的自动化中，这样可以每天定时运行。你也可以直接通过Siri呼出*
  
## 原理
   POST回放
   
  
  
  
   (希望有大佬能用python做出一个程序脚本来造福我们)
