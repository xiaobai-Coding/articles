你好，我是小白Coding日志，一个热爱技术的程序员。在这里，我分享自己在编程和技术世界中的学习心得和体会。希望我的文章能够给你带来一些灵感和帮助。欢迎来到我的博客，一起在技术的世界里探索前行吧！
### 前言
我们在日常工作中最痛苦的事情莫过于为自己的变量命名，取一个既有意义又符合规范的变量名有时确实令人费神例如一些文件命名、函数、CSS类名，而英语水平又有限，我就因为变量命名而烦恼、痛苦。相信很多人和我一样往往在这个时候会打开百度翻译，输入中文名称来翻译为英文。这种方式也不是不行，只是效率比较低下，首先你要打开百度翻译输入中文变量名称后等待返回翻译结果，然后将翻译结果复制粘贴到自己的VSCode中，再在VSCode中将英文变量修改为符合规范的变量，比如——驼峰命名，你为了翻译要频繁的切换窗口，还需要对翻译结果再进一步调整优化，这一过程也很浪费时间，尤其是在需要处理大量数据的时候这个问题会提现的更为明显。
### 提升效率的工具
> **工具存在的意义就是方便人们的工作生活**

#### var-translate-en
朋友，我推荐你赶紧扔掉传统的翻译方式吧！在VSCode插件中搜索var-translate-en并安装
![image.png](https://cdn.nlark.com/yuque/0/2024/png/36013995/1706073269587-aa19f7ff-027e-40b0-be44-d295beb9b1fe.png#averageHue=%23f9f7dc&clientId=u10a7947b-77d1-4&from=paste&height=393&id=vL1fv&originHeight=393&originWidth=342&originalType=binary&ratio=1&rotation=0&showTitle=false&size=17386&status=done&style=none&taskId=u8ca59aa6-bae9-4ba8-a5e6-f2945864be5&title=&width=342)
#### var-translate-en使用方法

1. 输入要翻译的内容
2. 选中需要翻译的内容
3. 按住Ctrl+Shift+V
4. 翻译后选择需要的命名风格即可

![image.png](https://cdn.nlark.com/yuque/0/2024/png/36013995/1706155481960-fa8317f6-7cf2-4c5b-be53-3cce972c84cc.png#averageHue=%23ececec&clientId=u10a7947b-77d1-4&from=paste&height=298&id=N525X&originHeight=298&originWidth=602&originalType=binary&ratio=1&rotation=0&showTitle=false&size=32960&status=done&style=none&taskId=u76100c95-ba0a-4ed0-988a-f80f9bcf4a3&title=&width=602)
#### 翻译服务配置
支持多个翻译服务平台（百度、腾讯、阿里、有道）一般来说配置一个就足够了
##### 百度翻译
以百度翻译为例进行配置如下步骤：

1. 访问百度翻译：[https://fanyi-api.baidu.com/](https://fanyi-api.baidu.com/) 并登陆账号
2. 选择通用文本翻译，点击立即使用，免费的就完全够用了
3. 注册并填写信息，选择个人开发者即可。

![image.png](https://cdn.nlark.com/yuque/0/2024/png/36013995/1706156527276-88d8d2e5-ff8e-43de-8d74-d0f039027f34.png#averageHue=%23fbfbfa&clientId=u10a7947b-77d1-4&from=paste&height=857&id=hcA8t&originHeight=857&originWidth=663&originalType=binary&ratio=1&rotation=0&showTitle=false&size=47518&status=done&style=none&taskId=ue8e41647-b6f0-4cd8-b4b9-99e57206c7b&title=&width=663)

4. 注册成功之后来到自己的管理控制台，就能看到APP ID和密钥对应的值

![image.png](https://cdn.nlark.com/yuque/0/2024/png/36013995/1706156643066-048980bf-c501-4167-ba2b-410239dfef04.png#averageHue=%2311100f&clientId=u10a7947b-77d1-4&from=paste&height=61&id=ioTkU&originHeight=61&originWidth=1292&originalType=binary&ratio=1&rotation=0&showTitle=false&size=12621&status=done&style=none&taskId=uccde14e0-ff46-46c8-8f09-967efd7f959&title=&width=1292)

5. 回到VSCode中点击打开设置面板并搜索 var-translate-en
6. 配置百度翻译APP ID和密钥，选择翻译服务为百度

![image.png](https://cdn.nlark.com/yuque/0/2024/png/36013995/1706157036809-383de69b-a39e-4757-833f-85a04cc4b59f.png#averageHue=%23c7ebcc&clientId=u10a7947b-77d1-4&from=paste&height=935&id=A76nh&originHeight=935&originWidth=1234&originalType=binary&ratio=1&rotation=0&showTitle=false&size=70277&status=done&style=none&taskId=u12870be8-2ed4-466d-a5d3-71b72b753bd&title=&width=1234)
经过以上的配置就可以愉快的使用翻译插件咯😁
还是那句话：**工具存在的意义就是方便人们的工作生活 **既然有这么好用的工具为什么不用呢
如果觉得有用，就给我点个赞吧😁
探索更多有趣知识，欢迎关注我的微信公众号！每天分享精彩内容，与你一同探寻知识的边界。扫码即可订阅，一起开启知识新旅程！🚀📚
![qrcode_for_gh_bd5bafbcdd40_258.jpg](https://cdn.nlark.com/yuque/0/2024/jpeg/36013995/1705556124681-b339e93e-c46c-41e7-9922-b49c58aeff21.jpeg#averageHue=%23a09f9f&clientId=u38add42d-4de3-4&from=ui&id=ufd2b1fe9&originHeight=258&originWidth=258&originalType=binary&ratio=1&rotation=0&showTitle=false&size=26790&status=done&style=none&taskId=u7f558f04-96e1-43f7-8d4c-70f1b40b037&title=)
关注我的技术博客，探索前沿科技与实用开发技巧。一起携手走向代码的精彩世界！🚀💻 不错过每一篇精彩！
> [https://www.xiaobaicoding.com/](https://www.xiaobaicoding.com/)



