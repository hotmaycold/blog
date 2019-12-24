## 原料
   
#### 1. 图床上传工具 [PicGo](https://github.com/Molunerfinn/PicGo) 
![](https://i.loli.net/2019/12/07/RajJCrT6FAEI173.png)

>写markdown文件最大的阻力其实就是图片没有一个方便稳定的图床，PicGo的快捷键和截图上传算是很顺手的了。 [使用文档](https://picgo.github.io/PicGo-Doc/zh/guide/)

#### 图床选择
[SM.MS](https://sm.ms/) 图床算是几年来比较稳定的了，而且**免费**虽然不知道大流量情况是否会影响响应速度，而且不知道图片会传到哪里，但用来存储不痛不痒的博客图片还是不错的，反正你也不常写。最重要的是PicGo给你设置好了，直接用就行了

![](https://i.loli.net/2019/12/07/e5h3LUfpPXCYn9R.png)

想安全有保障可以绑定自己的[七牛云对象存储](https://portal.qiniu.com/signup?code=1hgwcg9wg4hg2)，毕竟有每个月免费10G也是稳稳的够

##### PicGo各版本支持度：
- ~~`微博图床` v1.0~~ **微博图床从 2019 年 4 月开始进行防盗链，不建议继续使用**
- `七牛图床` v1.0
- `腾讯云 COS v4\v5版本` v1.1 & v1.5.0
- `又拍云` v1.2.0
- `GitHub` v1.5.0
- `SM.MS` v1.5.1
- `阿里云 OSS` v1.6.0
- `Imgur` v1.6.0

#### 2. 微信截图
Mac下微信截图快捷键为 `Command+Control+A`、QQ截图也行

#### 3. gif屏幕录制[LICEcap](https://www.cockos.com/licecap/)
![](https://i.loli.net/2019/12/07/3VlyUBwpNku6viJ.png)

屏幕录制转gif，体积还小，不夸张的说这个录制软件支持了我写博客

## 常规用法（SM.MS）

- 微信截图 `Command+Control+A` 然后回车图片已经到剪贴板了
- 查看PicGo上传快捷键 我设置的是 `Command+Shift+P`

![](https://i.loli.net/2019/12/07/MHbltTFBX3fh7nI.png)
![](https://i.loli.net/2019/12/07/HpdJvt6jQ1N5a9T.png)

- 上传以后链接就自动到了剪贴板了，但是因为我们要拷贝到markdown里，所以链接的格式得调整一下 `![SMMS]($url)`

![](https://i.loli.net/2019/12/07/M2B9W5qiNC4mxGn.png)
![](https://i.loli.net/2019/12/07/Uh4lo6BRes7DLH8.png)
![](https://i.loli.net/2019/12/07/PvcV7Ypno2C3WwL.png)

- 直接复制到vscode就完成了
![](https://i.loli.net/2019/12/07/otWhyMk9Riv1xjL.png)

## 常见问题
- sm.ms 限流一分钟只能传十张图
![](https://i.loli.net/2019/12/07/ifXpzTExqwBGedm.png)
- [偶发性的上传图片失败现象](https://github.com/Molunerfinn/PicGo/issues/311) 一般出现以下异常为网络异常
``` 
Error
  at Object.handle (/Applications/PicGo.app/Contents/Resources/app.asar/node_modules/picgo/dist/plugins/uploader/smms.js:42:19)
  at process._tickCallback (internal/process/next_tick.js:68:7)
-------Error Stack End-------
```




 

