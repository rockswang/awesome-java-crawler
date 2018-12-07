# awesome-java-crawler
本仓库收集整理Java爬虫相关资源

### 非浏览器Java爬虫框架
* [WebMagic](https://github.com/code4craft/webmagic) - Java垂直爬虫框架
* [crawler4j](https://github.com/yasserg/crawler4j) - 多线程爬虫框架
* [SeimiCrawler](https://github.com/zhegexiaohuozi/SeimiCrawler)
* [ispider](https://github.com/xpleaf/ispider) - 分布式爬虫框架
* [Gecco](https://github.com/xtuhcy/gecco) - 轻量化的易用的网络爬虫

### 基于浏览器核心的爬虫框架
* [Selenium](https://www.seleniumhq.org/) - 应用最广泛的浏览器自动化测试框架，支持所有主流浏览器
* [PhantomJS(javascript)](http://phantomjs.org/) - 基于WebKet核心的无头浏览器。已经停止维护
* [Puppeteer(javascript)](https://github.com/GoogleChrome/puppeteer/) - 提供基于Chrome开发工具协议控制Chrome浏览器的高层开发API
* [Chrome Devtools Protocol](https://github.com/ChromeDevTools/awesome-chrome-devtools) - Chrome开发工具协议相关资源
* [CDP4J](https://github.com/webfolderio/cdp4j) - Java版本的开发工具协议支持库。注意本库为商业授权
* [Tampermonkey](https://tampermonkey.net/) - 浏览器脚本管理器，也可用于浏览器自动化控制

### Java爬虫实例
* [知乎爬虫](https://github.com/wycm/zhihu-crawler) - 使用http代理，多线程
* [电商爬虫](https://github.com/JFanZhao/spider) - httpclient+hbase+solr+redis+zookeeper

### Java网络框架
* [java-curl](https://github.com/rockswang/java-curl) - CURL命令行工具的纯java实现，功能全面，特别适合爬虫
* httpclient - 历史悠久的Apache HTTP开源库
* okhttp - 目前流行的HTTP开源库，可用于Android
* retrofit - 基于okhttp的高层HTTP库，提供基于注解的API

### 请求应答解析
* [jsoup](https://jsoup.org/) - 网络请求，HTML解析，CSS Selector/xPath查询
* Jackson - JSON解析
* Gson - JSON解析
* [dom4j](https://dom4j.github.io/) - XML解析

### 代理IP
* [66免费代理网](http://www.66ip.cn/)
* [西刺免费代理IP](http://www.xicidaili.com/)
* [无忧代理](http://www.data5u.com/)
* [芝麻软件](http://www.zhimaruanjian.com/)

### 验证码破解
* [冷月JS爆破](https://github.com/leng-yue/Lengyue-Vcode/) - 各种滑动验证码识别
* [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) - 开源OCR引擎，可用于自动识别较简单的图片验证码
* [若快](http://www.ruokuai.com/) - 人肉打码平台，服务较稳定，应答时间较快

### 抓包分析，请求拦截等工具
* [Fiddler](https://www.telerik.com/fiddler) - Windows平台上常用抓包工具，可以分析HTTPS，可C#编程自行扩展
* Charles - Mac上可用的抓包工具
* [LittleProxy-MITM](https://github.com/ganskef/LittleProxy-mitm) - 基于LittleProxy，可编程扩展的Java代理服务器
* [proxyee](https://github.com/monkeyWie/proxyee) - 国人作品，支持HTTPS代理

### 页面Javascript跟踪分析
* [javascript-breakpoint-collection](https://github.com/mattzeunert/javascript-breakpoint-collection) - 一个Chrome插件，可用于设定高级断点；也可以直接在控制台执行其源码，之后即可在控制台设断点，可以监听任意对象属性读写、cookie读写等
* [从javascript脚本混淆说起](https://www.freebuf.com/articles/system/140062.html)
* [几种常见的JavaScript混淆和反混淆工具分析实战](https://www.freebuf.com/articles/web/97945.html)

### 其它工具
* CURL - 最常用的命令行请求模拟工具，Windows下可以通过Cygwin安装，也可以直接用java-curl
* [HTTPBIN.ORG](https://httpbin.org) - 一个网站，可根据需求模拟各种HTTP应答，也可用于验证代理的匿名性（透明/匿名/高匿）
  * ```curl -x <proxy>:<port> https://httpbin.org/get?show_env=1``` - 如果X-Forwarded-For和origin不一致，表明使用了非匿名代理
* [淘宝IP地址库](http://ip.taobao.com/)
  * ```http://ip.taobao.com/service/getIpInfo.php?ip=11.206.34.204``` - 查询给定IP的归属地
  * ```curl http://ip.taobao.com/service/getIpInfo2.php -x <proxy>:<port> -d "ip=myip"``` - 查询当前主机的公网IP归属地，这个命令可以验证代理IP是否可用
* [IP138](http://ip138.com) - 查询IP归属地、手机号段等
* [在线UA库](https://developers.whatismybrowser.com/useragents/explore/software_name/) - 各种真实浏览器UserAgent列表
* WEB前端助手 - Chrome插件，提供大量实用工具，如JSON格式化，编解码等

### 参考和资源
#### 概念与思路
* [网络爬虫干货总结](https://juejin.im/post/5bce8201518825773605597d) - 虽然是python栈的，但是对爬虫各个环节的概念总结的非常全面
* [Java 月薪25K的爬虫工程师对爬虫的流程做了一个非常全面的总结！](https://blog.csdn.net/Knight_VIP/article/details/81736918) - 膜拜ing...
* [那些年绕过的反爬手段](https://www.freebuf.com/articles/web/166125.html)
* [反反爬虫手段收集](https://github.com/luyishisi/Anti-Anti-Spider)
#### Chrome浏览器相关
* [Chrome命令行参数列表](https://peter.sh/experiments/chromium-command-line-switches/) - 定制化chrome，比如启动无头版浏览器
* [Getting Started with Headless Chrome](https://developers.google.com/web/updates/2017/04/headless-chrome) - 介绍如何使用无头版Chrome
* [CentOS6上安装Chrome](https://intoli.com/blog/installing-google-chrome-on-centos/) - 用于搭建无头浏览器爬虫生产环境
* [CentOS 7.x环境下搭建: Headless chrome + Selenium + ChromeDriver](https://blog.csdn.net/zhuyiquan/article/details/79537623)
* [apkmirror](https://www.apkmirror.com/apk/google-inc/chrome/variant-%7B%22arches_slug%22%3A%5B%22x86%22%5D%7D/) - 安卓x86版Chrome下载，可用于安卓模拟器
#### Android逆向相关：xposed等
* [思路分享 | 看我如何给微信下钩子](https://www.freebuf.com/articles/web/156944.html)
