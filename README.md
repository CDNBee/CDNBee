# CDNBee

<a href="http://cdnbee.com">CDNBee.com</a> 的目标是提供这样一个仓库，让它尽可能全面收录优秀的开源库，并免费为之提供 CDN 加速服务，使之有更好的访问速度和稳定的环境。同时，我们也提供开源库源接入的入口，让所有人都可以提交开源库，包括 JavaScript、CSS、IMG 和 swf 等静态文件。

# 如何提交开源库

http://cdnbee.com/pr

<pre>
.
├── jquery                    # ... 库名
│   ├── 1.8.3                 # ... 版本号
│   |   └── jquery.min.js     # ... 文件名，不带版本
│   └── 1.9.1
│       └── jquery.min.js
└── package.json              # ... 最新版本文件的描述
</pre>

# 更新开源库

理论上我们自动更新库的版本文件，并且不会删除旧版本，但如果你在 <a href="http://cdnbee.com">CDNBee.com</a> 找不到最新的版本，则可以通过往该库中添加一个版本目录，并且修改相应的 package.json 文件，利用 Pull Request 来提醒我们。

# 使用注意

虽然大多数库都是基于 MIT / BSD License 开源的，但在有某些库在个人/商业应用上是有区别的，比如 Highcharts 这个库，所以请大家在使用这些库的时候，最好能点击其网站、代码仓库（在搜索结果中有链接）中查看其开源协议。

# 作者和服务商

维护者：

<a href="https://github.com/helantao">Henry</a>

<a href="https://github.com/iamnat">NAT</a>

此仓库由国内优秀的云存储服务商 <a href="https://qiniu.com">七牛云存储</a> 提供存储和加速赞助。同步国外 <a href="https://github.com/cdnjs/cdnjs">CDNJS</a> 源站，同时由国内开源贡献值提交其它有价值的库。感谢所有开源库作者和挖掘者的努力。

