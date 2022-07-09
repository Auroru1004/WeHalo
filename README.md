[![](https://raw.githubusercontent.com/aquanlerou/WeHalo/master/image/wehalo.jpg)](https://github.com/aquanlerou/WeHalo)

## WeHalo 支持最新版本 Halo

大家的支持，鼓励，认可，是我坚持开源的动力，虽然后面开发完有点拖拉，请原谅 ~ 渲染图在设计中

后续更多功能开发并开发给大家使用，新版本 **WeHalo** 会存在不少问题欢迎大家多给我提 **Issues** 我会尽快处理

新版本使用的问题不懂可以通过小程序联系作者找到我或者添加``QQ交流群: 260050047 / 559856207``

> ✍ Halo 一款现代化的个人独立博客系统 [Halo](https://halo.run)

[![Github](https://img.shields.io/badge/Author-Aquan-FF4500.svg?style=flat-square)](https://github.com/aquanlerou)
[![GitHub release](https://img.shields.io/github/release/aquanlerou/WeHalo.svg?style=flat-square)](https://github.com/aquanlerou/WeHalo/releases)
[![](https://img.shields.io/github/languages/code-size/aquanlerou/WeHalo.svg?style=flat-square)](https://github.com/aquanlerou/WeHalo)
[![GitHub LICENSE](https://img.shields.io/github/license/aquanlerou/WeHalo.svg?style=flat-square)](https://github.com/aquanlerou/WeHalo/blob/master/LICENSE)
[![star](https://img.shields.io/github/stars/aquanlerou/WeHalo.svg?label=Stars&style=social)](https://github.com/aquanlerou/WeHalo)
[![star](https://gitee.com/aquanrun/WeHalo/badge/star.svg?theme=white)](https://gitee.com/aquanrun/WeHalo/stargazers)

------------------------------

<details><summary>目录</summary>

- [简介](#简介)
- [快速开始](#快速开始)
- [文档](#文档)
- [演示](#演示)
- [许可证](#许可证)
- [后续功能](#后续功能)
- [感谢](#感谢)
- [捐赠](#捐赠)

</details>

## 简介

**WeHalo** [wiˈheɪloʊ]，意为我们的光环，嘻嘻。

配合 [**Halo**](https://github.com/halo-dev/halo) 轻快，简洁，功能强大的博客系统而开发出来的 **简约风** 微信小程序版博客

> QQ交流群: 260050047 / 559856207

## 快速开始

**注：开源不易请留 WeHalo 底部署名不要删除**

```bash
git clone https://github.com/aquanlerou/WeHalo.git
```

代码下载后，把 **image** 文件夹删除（放的是README中的图片与项目无关），用小程序 IDE 打开后即可使用。

**注：请选择小程序项目，非小游戏，例子中无 appid，所以无法在手机上运行，如果需要真机调试，请在打开例子时，填上自己的小程序 id**


## 文档

修改``app.js``文件的全局变量，改为你的 **Halo** 博客的地址，请更新最新的 **Halo** 配合使用

**注：必须是HTTPS的因为，微信官方规定，还有把你的博客地址``如：https://aquan.run``和``https://v2.jinrishici.com``添加到微信公众平台的 ``request 合法域名``中**

```
globalData: { //全局变量
        userInfo: null,
        skin: null,
        roleFlag: false,
        BlogName: "爱敲代码的猫",//博客名字
        url: "https://aquan.run",//博客地址（需HTTPS）
        token: "",//Halo博客后台设置
        highlightStyle: "dracula",//代码高亮样式，可用值default,darcula,dracula,tomorrow
        adminOpenid: "ogogn47AhczrMBgcTCPbUwugqLcU",//导入项目后可以在Console中看到  openidCloudResult: xxxxxxx  (xxx就是adminOpenid)
        HaloUser: "xx",//Halo后台用户名
        HaloPassword: "xx",//Halo后台密码
 }
```

**注：
关于新版本 ``WeHalo`` 找不到 ``adminOpenid`` 的处理方法： ``https://gitee.com/aquanrun/WeHalo/issues/I12J1G``**

设置个人专属**Logo** 修改 ``WeHalo\miniprogram\colorui\main.wxss`` 文件最后面的

``` 
.home-img{
    padding: 24rpx;
    background-repeat: no-repeat;
    background-size: contain;
    /* background-image:url(../image/cat.png); */
    background-image:url('xxxxx');//logo图片地址
}
```


html2wxml插件版本准备

> 1. 添加插件
![添加小程序插件](https://www.qwqoffice.com/html2wxml/images/plugin-1.png "添加小程序插件")
> 2. 搜索 `html2wxml` ，选中并添加
![添加小程序插件](https://www.qwqoffice.com/html2wxml/images/plugin-2.png "添加小程序插件")
> 3. 添加成功
![添加小程序插件](https://www.qwqoffice.com/html2wxml/images/plugin-3.png "添加小程序插件")


> 文档正在不断完善中，遇到问题请加群提问或者 [**Issues**](https://github.com/aquanlerou/WeHalo/issues) 等你吐槽...


## 演示

![WeHalo](https://github.com/aquanlerou/WeHalo/blob/master/image/wx.png)

#### [**更多演示**](https://github.com/aquanlerou/WeHalo/issues/53)


## 许可证

[![GitHub LICENSE](https://img.shields.io/github/license/aquanlerou/WeHalo.svg?style=flat-square)](https://github.com/aquanlerou/WeHalo/blob/master/LICENSE)

> WeHalo使用GPL-v3.0协议开源，请尽量遵守开源协议，即便是在中国。

## 功能

- [x] 重新设计**WeHalo**
- [x] 自定义导航栏（个人觉得好看可自定义）
- [x] 个人名片（可宣传自己）
- [x] 博文展示
- [x] 评论展示
- [x] 搜索文章功能
- [x] 文章评论功能
- [x] 博主查看评论功能
- [x] 博主回复评论功能
- [x] 评论功能内容识别
- [x] 友链展示
- [x] 日记本
- [ ] 点赞功能（云函数）
- [ ] 文章浏览统计功能（云函数）
- [ ] 用户回复评论追评功能
- [ ] 生成海报（微信朋友圈装X）
- [x] 图库展示([小熊随笔](https://www.xtyu.top/)贡献开发)
- [x] 图库图片上传([小熊随笔](https://www.xtyu.top/)贡献开发)
- [x] 短视频去水印([小熊随笔](https://www.xtyu.top/)贡献开发)
- [x] 按类别导航([小熊随笔](https://www.xtyu.top/)贡献开发)
- [x] 加密分类限制([小熊随笔](https://www.xtyu.top/)贡献开发)
- [ ] 想到就写...

## 感谢

WeHalo的诞生离不开下面这些项目的支持：

- **[Halo](https://github.com/halo-dev/halo)： 一个优秀的开源博客发布应用。**
- **[ColorUI](https://github.com/weilanwl/ColorUI)：鲜亮的高饱和色彩，专注视觉的小程序组件库**
- **[iView Weapp](https://github.com/TalkingData/iview-weapp)：一套高质量的微信小程序 UI 组件库**
- **[Painter](https://github.com/Kujiale-Mobile/Painter)：微信小程序生成图片库，绘制一张可以发到朋友圈的图片**
- **[html2wxml](https://github.com/qwqoffice/html2wxml)：用于微信小程序的HTML和Markdown格式的富文本渲染组件，支持代码高亮**
- **[一言·古诗词](https://github.com/xenv/gushici)：Hitokoto API，随机返回一条古诗词名句。采用 Vert.x + Redis 全异步开发，毫秒级稳定响应。**

[![](https://raw.githubusercontent.com/savingrun/WeHalo/master/image/logo-jb.svg)](https://www.jetbrains.com)

> 
> 各位的哇哈哈，再次感谢各位的支持
> 

## Stargazers over time
[![Stargazers over time](https://starchart.cc/aquanlerou/WeHalo.svg)](https://starchart.cc/aquanlerou/WeHalo)

## Thanks to all the people who already contributed!

<a href="https://github.com/savingrun/WeHalo/graphs/contributors">
  <img src="https://contributors-img.web.app/image?repo=savingrun/WeHalo" />
</a>
