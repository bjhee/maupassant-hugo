# Maupassant
Maupassant theme, ported to Hugo.

Fork from [rujews/maupassant-hugo](https://github.com/rujews/maupassant-hugo)

You can refer to the site [Billy.J.Hee](http://www.bjhee.com)

## Additional Functions

1. Replace Google Search by Baidu Search
1. Adding Register Info (aka 备案 in China) at footer.  You can add `registerInfo="<register_number>"` in `[params]` section of config.toml or config.yaml
1. Add `related` option in `[params]`, enable "See Also" function when setting it to true, default is false
1. Add `recentPostNumber` option in `[params]`, it can specify the number of links listed on "Recent Post" section of side bar, default is 10
1. Blog list only contains "type: post" type articles
1. Add Baidu Analysis, need to find the embedded script of Baidu, and config the id in "hm.src" url

## Sample Configuration

```toml
baseURL = "http://www.bjhee.com/"
languageCode = "en"
title = "Billy.J.Hee"
hasCJKLanguage = true
theme = "maupassant-hugo"
enableRobotsTXT = true
PaginatePath = "page"
summaryLength = 140

[author]
    name = "Billy.J.Hee"
    homepage = "http://www.bjhee.com/"

[params]
    subtitle = "Billy.J.Hee Blog Site"
    description = "Billy.J.Hee Blog Site"
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
    name = "Billy.J.Hee Github"
    url = "https://github.com/bjhee/"
    title = "Billy.J.Hee Github"

[[menu.main]]
    identifier = "archives"
    name = "Archives"
    url = "/archives/"
    weight = 3

[[menu.main]]
    identifier = "about"
    name = "About"
    url = "/about/"
    weight = 4
```
