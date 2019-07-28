# Maupassant
Maupassant theme, ported to Hugo.

Fork from [rujews/maupassant-hugo](https://github.com/rujews/maupassant-hugo)

参加站点：[思诚之道](http://www.bjhee.com)

## 附加功能

1. 将Google搜索改为百度搜索
1. 页脚添加备案号，在config.toml（或config.yaml）的`[params]`项中添加 `registerInfo="<备案号>"`即可
1. 添加`[params]`里的选型`related`，设为true则开启文章底部"See Also"功能，false则关闭，默认关闭
1. 添加`[params]`里的选型`recentPostNumber`，设置右边栏最近文章链接的个数，默认为10
1. 博客列表只留"type: post"类型的文章
1. 添加百度统计，需要在百度统计的嵌入脚本里，找到"hm.src"地址，并把后面的那串ID配上

## 配置示例

```toml
baseURL = "http://www.bjhee.com/"
languageCode = "zh-cn"
title = "思诚之道"
hasCJKLanguage = true
theme = "maupassant-hugo"
enableRobotsTXT = true
PaginatePath = "page"
summaryLength = 140

[author]
    name = "Billy.J.Hee"
    homepage = "http://www.bjhee.com/"

[params]
    subtitle = "Billy.J.Hee的博客"
    description = "Billy.J.Hee的博客"
    keywords = "Blog"
    toc = true
    related = false
    recentPostNumber = 5
    baiduAnalysisId = "0f4fc19c9df1256edcd8e4f84e045f78"
    registerInfo = "沪ICP备xxxx号"
    customCSS = ["style.extra.css"]
    customJS = ["app.extra.js"]

[params.utteranc]
    repo = "bjhee/comments"
    issueTerm = "url"
    theme = "github-light"

[[params.links]]
    name = "Billy.J.Hee的Github"
    url = "https://github.com/bjhee/"
    title = "Billy.J.Hee的Github"

[[menu.main]]
    identifier = "archives"
    name = "存档"
    url = "/archives/"
    weight = 3

[[menu.main]]
    identifier = "about"
    name = "关于"
    url = "/about/"
    weight = 4
```