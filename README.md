# CDNBee

<a href="http://cdnbee.com" target="_blank">CDNBee.com</a> 的目标是提供这样一个仓库，让它尽可能全面收录优秀的开源库，并免费为之提供 CDN 加速服务，使之有更好的访问速度和稳定的环境。同时，我们也提供开源库源接入的入口，让所有人都可以提交开源库，包括 JavaScript、CSS、图片和 swf 等静态文件。

# 如何提交开源库

Fork 这个仓库，在 static/ 下新建一个目录，这个目录下可以有多个版本（至少一个版本）如：
.
├── jquery                    # ... 库名
│   ├── 1.8.3                 # ... 版本号
│   |   └── jquery.min.js     # ... 文件名，不带版本
│   └── 1.9.1
│       └── jquery.min.js
└── package.json              # ... 最新版本文件的描述

编辑 package.json 描述文件，这个文件描述最新版本的信息。具体写法请参照：static/typo.css/package.json

{
  // 这三项让你的文件能正常被索引到
  // 项目名要与文件夹名一致
  "name": "项目名",
  "filename": "主文件名，比如 XYZ.js",
  "version": "1.0",

  // 其他
  "description": "项目简介",
  "homepage": "项目主页，如 http://cdnbee.com",
  "keywords": [],
  "maintainers": [
    {
      "name": "作者/维护者",
      "web": "http://cdnbee.com",
      "mail": "example@example.com"
    }
  ],
  "repositories": [
    {
      // svn 等
      "type": "git",
      "url": "https://github.com/cdnbee/static"
    }
  ]
}

然后给这个仓库提交 Pull Request。理论上我们会用最快的速度验证、审核这个库。一旦 Pull Request 被 Merge，则马上可以能过 CDN 访问。

为了保证存放在 <a href="http://cdnbee.com" target="_blank">CDNBee.com</a> 上开源库的质量，我们建议提交的仓库有一定的关注度（包括Github的star，其他仓库平台的收藏数量等可参考数值），目前建议这个数量在30以上。

# 更新开源库

理论上我们自动更新库的版本文件，并且不会删除旧版本，但如果你在 <a href="http://cdnbee.com" target="_blank">CDNBee.com</a> 找不到最新的版本，则可以通过往该库中添加一个版本目录，并且修改相应的 package.json 文件，利用 Pull Request 来提醒我们。

# 使用注意

虽然大多数库都是基于 MIT / BSD License 开源的，但在有某些库在个人/商业应用上是有区别的，比如 Highcharts 这个库，所以请大家在使用这些库的时候，最好能点击其网站、代码仓库（在搜索结果中有链接）中查看其开源协议。

# 作者和服务商

维护者：<a href="https://github.com/helantao" target="_blank">Henry</a>

此仓库由国内优秀的云存储服务商 <a href="https://qiniu.com" target="_blank">七牛云存储</a> 提供存储和加速赞助。同步国外 CDNJS 源站，同时由国内开源贡献值提交其它有价值的库。感谢所有开源库作者和挖掘者的努力。
