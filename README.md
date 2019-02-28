# FakeScreenshot
> 对抗假新闻系列项目之一：截屏 = 实锤？相信你就输了！



#### 写在前面

---

如果有一天你在群里看到这么一张图，你第一反应是什么？

![微博截图](https://ww1.sinaimg.cn/large/007i4MEmgy1g0jrh5ez40j30h2045t91.jpg)

“卧槽，这么快？”

“正好这段时间没事做，学一下”

“和2.0有什么区别啊？”

“求你们别更了，我学不动了.jpg ？”

"支持TS吗？"

**不管怎样，只要第一反应不是怀疑其真实性，那么你就是“假截图”的受害者！**



我们都曾看到过各种截屏：包括不限于`知乎`、`微博`、`豆瓣`、`NGA`、`V2EX`、`QQ`、`微信` 、`各种新闻站`...

如果那些截屏内容只涉及到段子还好，但多数情况不是。它们往往和某事/某人有关，这（假截图）就**极有可能**导致人们对该事/人产生错误的看法（之所以说错误，是因为我认为**大多数**假截图的制作者都怀有不良动机。）

另外，**多数人并不会去主动验证该截图描述事情的真伪**（不这么做的原因这里不做讨论），这是“假截图”泛滥的重要原因之一。

**对此我们能做什么呢？**

三个方向：1. 阻止传播（极难实现）2. 告诉人们应该主动去求证（很难实现）3. 至少告诉人们首先应该持怀疑态度（有些可能性）。

我选择了第三个方向。而方法呢，我选择反其道而行之，开发一个**帮助人们非常简单地制作常见网站、软件的虚假截图（当然，内容可以由用户自定义）** 的网站（针对QQ、微信等手机软件的虚假截图制作，我们也考虑开发一款App）。

**通过本项目制作出来的假截图的传播来告诉人们这样一件事：“哦，原来各大网站/App的截图都可以造假啊！”**

> 后期如何传播我们的“造假”网站？
>
> 我们项目制作出来假截图时，可以在右下角添加一个“非常不明显”的水印来指向我们的“造假”网站

那么你说下一次，这个人再看到这种截图的时候，他会不会第一时间对内容保持怀疑呢？



#### FAQ

---

**假截图就全是不好的吗？**

答案当然是否定的。另外，这类问题实在没什么意义，因为这个世界上就没有几件能 “100%肯定” 的事情。（建议尽早摒弃这种“非此即彼”的极端思想，于人生无益）

**这个项目的意义在哪里？**

告诉人们看到任何截图的时候都应该保持怀疑。

**我不会Vue，只会React/Angular可以参与吗？**

我选择某个技术栈的原因只是想确保一点，项目能进行下去，因为我会Vue、React、ReactNative，使用这三个技术栈，我能把项目推进下去（因为很可能大多数代码都是我来写 🤣 ）所以就不考虑Angular了。

所以你只要掌握Vue（现在项目是Vue，看有没有人参与吧，再讨论要不要换React）、React、ReactNative中的任一项，都可以参与进来。



#### 预览

---

**（刚开始开发，只完成了“简单版微博”部分）：https://fakes.netlify.com/**

![预览](http://wx2.sinaimg.cn/large/006fVPCvly1g0jvjz7fmyj30je0bpwf3.jpg)

#### 技术栈

------

> 涉及的技术很少，而且难度不高；
>
> 纯前端项目，完全不涉及后端逻辑；
>
> 人手充足的话考虑同时开发App端（iOS、Android（技术栈的话，可以考虑ReactNative））

- Vue
- html2canvas



#### 如何贡献代码

------

**须知：** 参与开发需要你了解基本`Git`技能（关键词：Git分支、提交Merge Request）

1. 联系我加入Organization：TheGreatJavaScript
2. 新建分支：以你的Github名称来命名
3. 开发：在你的分支开发，然后发起Merge Request

项目开发群：792410430 （仅限已经或者将要为项目**贡献代码**的开发者加入！）

> 具体代码规范不着急，有人参与的话我再补充



#### 如何运行

---

确保你本地有Vue开发环境

```bash
git clone git@github.com:thegreatjavascript/FakeScreenshot.git
cd FakeScreenshot
yarn // or cnpm i
yarn run dev // or npm run dev
```

浏览器打开：http://localhost:8080



#### 待办事项

---

- [ ] 知乎页面简单版
- [ ] 微博版支持名称右侧添加/删除 各种标志（比如vip1、2、3级的标志，黄色V标志）（这些标志的图片转换成base64存到JSON文件中）
- [ ] 微博版正文中支持添加/删除图片（图片暂时只支持一张；视频先不考虑）（图片像微博一样支持两种形态，缩放和点击后放大）
- [ ] 微博版支持添加表情；
- [ ] 微博版支持 @某用户 的字体变色（和微博一样是#eb7350）
- [ ] 微博版支持转载
- [ ] 水印：编辑时的页面背景上也要添加水印，避免有人直接用其他截图工具直接截图。
- [ ] 水印：水印如何添加让其他人难以消除
