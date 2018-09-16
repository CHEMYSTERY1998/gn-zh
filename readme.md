# gn [![translate-svg]][translate-list] 

[translate-svg]: http://llever.com/translate.svg
[translate-list]: https://github.com/chinanf-boy/chinese-translate-list

「 GN是一个元构建系统,可以为[ninja](https://ninja-build.org)生成构建文件. 」

[中文](./readme.md) | [english](https://gn.googlesource.com/gn/)


---

## 校对 🀄️

<!-- doc-templite START generated -->
<!-- docTempliteId = 'google' -->
<!-- repo = 'gn' -->
<!-- repo = 'gn' -->
<!-- commit = '77d64a3da6bc7d8b0aab83ff7459b3280e6a84f2' -->
<!-- time = '2018 9.16' -->
翻译的原文 | 与日期 | 最新更新 | 更多
---|---|---|---
[commit] | ⏰ 2018 9.16 | [googlesource] | [中文翻译][translate-list]

> 需要翻墙

[googlesource]: https://.googlesource.com/gn/+/master
[commit]: https://.googlesource.com/gn/+/77d64a3da6bc7d8b0aab83ff7459b3280e6a84f2
<!-- doc-templite END generated -->

- [ ] [readme](./readme.md)
- [ ] [docs](./docs) 0/8

### 贡献

欢迎 👏 勘误/校对/更新贡献 😊 [具体贡献请看](https://github.com/chinanf-boy/chinese-translate-list#贡献)

## 生活

[help me live , live need money 💰](https://github.com/chinanf-boy/live-need-money)

---

### 目录

<!-- START doctoc -->
<!-- END doctoc -->


# GN

GN是一个元构建系统,可以为[ninja](https://ninja-build.org)生成构建文件.有文件[文档/](./docs).

## 入门

```
git clone https://gn.googlesource.com/gn
cd gn
python build/gen.py
ninja -C out
# To run tests:
out/gn_unittests
```

在Windows上,它是预期的`cl.exe`,`link.exe`,和`lib.exe`可以找到`PATH`,因此您需要从Visual Studio命令提示符或类似命令运行.

在Linux和Mac上,默认编译器是`clang++`,最近的版本预计将在`PATH`.这可以通过设置覆盖`CC`,`CXX`,和`AR`.

## 发送补丁

GN使用[格里特](https://www.gerritcodereview.com/)用于代码审查.如何修补的简短版本是:

```
Register at https://gn-review.googlesource.com.

... edit code ...
ninja -C out && out/gn_unittests
```

然后,上传更改以供审核:

```
git commit
git cl upload --gerrit
```

修改更改时,请使用:

```
git commit --amend
git cl upload --gerrit
```

这将添加新的更改到现有的代码审查,而不是创建一个新的.

我们要求所有贡献者[签署Google的贡献者许可协议](https://cla.developers.google.com/)(根据需要选择个人或公司,选择"任何其他Google项目").

## 社区

您可以提出问题,并跟随GN的开发在Chromium上进行[GN-dev的@](https://groups.google.com/a/chromium.org/forum/#!forum/gn-dev)谷歌集团.
