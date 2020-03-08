# 搜索链接门户

为了方便直接进行搜索（而不用二次跳转），给出各网站搜索链接

有 {query} 的 Url 为 GET Request，直接将 {query} 换为需要搜索的内容即可（一般中英文都可）。Alfred 列中连接为 Alfred web search share link。

无 {query} 的 Url 不支持 GET Request，需要打开网页后在表单处填写。Alfred workflow 文件夹中提供了 Alfred Workflow 通过 Javascript 模拟搜索。

最新列表和 Workflow 可以在 [Github](https://github.com/zhengzangw/Portal-of-Search) 上获得

## 通用

|        | Alfred                                                                                                                                                     | Url                                                 |
| ------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 微博   | [s](alfred://customsearch/Search%20Weibo%20for%20%27%7Bquery%7D%27/s/utf8/nospace/https%3A%2F%2Fs.weibo.com%2Fweibo%3Fq%3D%7Bquery%7D%26Refer%3Dindex)     | https://s.weibo.com/weibo?q={query}&Refer=index     |
| 百度   | [s](alfred://customsearch/Search%20Baidu%20for%20%27%7Bquery%7D%27/s/utf8/nospace/https%3A%2F%2Fwww.baidu.com%2Fs%3Fwd%3D%7Bquery%7D)                      | https://www.baidu.com/s?wd={query}                  |
| 知乎   | [s](alfred://customsearch/Search%20Zhihu%20for%20%27%7Bquery%7D%27/s/utf8/nospace/https%3A%2F%2Fwww.zhihu.com%2Fsearch%3Ftype%3Dcontent%26q%3D%7Bquery%7D) | https://www.zhihu.com/search?type=content&q={query} |
| Quara  | [s](alfred://customsearch/Search%20Quora%20for%20%27%7Bquery%7D%27/s/utf8/nospace/https%3A%2F%2Fwww.quora.com%2Fsearch%3Fq%3D%7Bquery%7D)                  | https://www.quora.com/search?q={query}              |
| Google | s                                                                                                                                                          | https://www.google.com/search?q={query}             |
| Bing   | s                                                                                                                                                          | https://cn.bing.com/search?q={query}                |
| reddit | [forum](alfred://customsearch/Search%20reddit%20for%20%27%7Bquery%7D%27/forum/utf8/nospace/https%3A%2F%2Fwww.reddit.com%2Fsearch%2F%3Fq%3D%7Bquery%7D)     | https://www.reddit.com/search/?q={query}            |

## 词条

|          | Alfred                                                                                                                                                                                  | Url                                                        |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| 维基     | wiki                                                                                                                                                                                    | https://zh.wikipedia.org/wiki/Special:Search/{query}       |
| MBA 智库 | [wiki](alfred://customsearch/Search%20MAB%E6%99%BA%E5%BA%93%20for%20%27%7Bquery%7D%27/wiki/utf8/nospace/https%3A%2F%2Fwiki.mbalib.com%2Fwiki%2FSpecial%3ASearch%3Fsearch%3D%7Bquery%7D) | https://wiki.mbalib.com/wiki/Special:Search?search={query} |

## 书籍

|              | Alfred                                                                                                                                                                                                                                             | Url                                                                                                                |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Genesis 书库 | [book](http://gen.lib.rus.ec/search.php?req={query}&open=0&res=25&view=simple&phrase=1&column=def)                                                                                                                                                 | http://gen.lib.rus.ec/search.php?req={query}&open=0&res=25&view=simple&phrase=1&column=def                         |
| 全国图书馆   | [book](alfred://customsearch/Search%20%E5%85%A8%E5%9B%BD%E5%9B%BE%E4%B9%A6%E9%A6%86%20for%20%27%7Bquery%7D%27/book/utf8/nospace/http%3A%2F%2Fbook.ucdrs.superlib.net%2Fsearch%3Fsw%3D%7Bquery%7D%26ecode%3Dutf-8%26channel%3Dsearch%26Field%3Dall) | http://book.ucdrs.superlib.net/search?sw=%E7%AE%97%E6%B3%95%E5%AF%BC%E8%AE%BA&ecode=utf-8&channel=search&Field=all |
| 豆瓣读书     | [book](https://search.douban.com/book/subject_search?search_text={query})                                                                                                                                                                          | https://search.douban.com/book/subject_search?search_text={query}                                                  |
| 鸠摩搜书     | book                                                                                                                                                                                                                                               | https://www.jiumodiary.com/                                                                                        |
| Pansoso      | [book](https://www.pansoso.com/zh/{query})                                                                                                                                                                                                         | https://www.pansoso.com/zh/{query}                                                                                 |

## 音乐

|        | Alfred                                                                                                                                                                        | Url                                                |
| ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------- |
| 网易云 | [music](alfred://customsearch/search%20Netease%20Music%20for%20%7Bquery%7D/music/utf8/nospace/https%3A%2F%2Fmusic.163.com%2F%23%2Fsearch%2Fm%2F%3Fs%3D%7Bquery%7D%26type%3D1) | https://music.163.com/#/search/m/?s={query}&type=1 |

## 文献

|                | Alfred                                                                                                                                                                                                               | Url                                             |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| Sci-hub        | [doi](alfred://customsearch/Search%20essay%20of%20DOI%3A%20%27%7Bquery%7D%27%20on%20sci-hub/doi/utf8/nospace/https%3A%2F%2Fsci-hub.se%2F%7Bquery%7D)                                                                 | https://sci-hub.se/{query}                      |
| dx.doi.org     | [doi](alfred://customsearch/Search%20essay%20of%20DOI%3A%20%7Bquery%7D/doi/utf8/nospace/http%3A%2F%2Fdx.doi.org%2F%7Bquery%7D)                                                                                       | http://dx.doi.org/{query}                       |
| Google Scholar | [essay](alfred://customsearch/Search%20Google%20Scholar%20for%20essay%20%27%7Bquery%7D%27/essay/utf8/nospace/https%3A%2F%2Fscholar.google.com%2Fscholar%3Fq%3D%7Bquery%7D)                                           | https://scholar.google.com/scholar?q={query}    |
| 谷歌学术镜像-1 | [essay](alfred://customsearch/Search%20%E8%B0%B7%E6%AD%8C%E5%AD%A6%E6%9C%AF%E9%95%9C%E5%83%8F-1%20for%20essay%20%27%7Bquery%7D%27/essay/utf8/nospace/https%3A%2F%2Fs3.sci-hub.org.cn%2F%2Fscholar%3Fq%3D%7Bquery%7D) | https://s3.sci-hub.org.cn//scholar?q={query}    |
| 谷歌学术镜像-2 | [essay](alfred://customsearch/Search%20%E8%B0%B7%E6%AD%8C%E5%AD%A6%E6%9C%AF%E9%95%9C%E5%83%8F-2%20for%20essay%20%27%7Bquery%7D%27/essay/utf8/nospace/https%3A%2F%2Fxueshu.123admin.com%2Fscholar%3Fq%3D%7Bquery%7D)  | https://xueshu.123admin.com/scholar?q={query}   |
| CNKI           | [essay](alfred://customsearch/Search%20CNKI%20for%20essay%20%27%7Bquery%7D%27/essay/utf8/nospace/http%3A%2F%2Fscholar.cnki.net%2Fresult.aspx%3Fq%3D%7Bquery%7D)                                                      | http://scholar.cnki.net/result.aspx?q={query}   |
| 维普           | [essay](alfred://customsearch/Search%20%E7%BB%B4%E6%99%AE%20for%20essay%20%27%7Bquery%7D%27/essay/utf8/nospace/http%3A%2F%2Fwww.cqvip.com%2Fmain%2Fsearch.aspx%3Fk%3D%7Bquery%7D)                                    | http://www.cqvip.com/main/search.aspx?k={query} |

## 商城

|                | Alfred                                                                                                                                                                                | Url                                                            |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| 京东           | [buy](alfred://customsearch/Buy%20%22%7Bquery%7D%22%20on%20%E4%BA%AC%E4%B8%9C/buy/utf8/nospace/https%3A%2F%2Fsearch.jd.com%2FSearch%3Fkeyword%3D%7Bquery%7D%26enc%3Dutf-8)            | https://search.jd.com/Search?keyword={query}&enc=utf-8         |
| 淘宝           | [buy](alfred://customsearch/Buy%20%22%7Bquery%7D%22%20on%20%E6%B7%98%E5%AE%9D/buy/utf8/nospace/https%3A%2F%2Fs.taobao.com%2Fsearch%3Fq%3D%7Bquery%7D)                                 | https://s.taobao.com/search?q={query}                          |
| 当当           | [buy](alfred://customsearch/Buy%20%22%7Bquery%7D%22%20on%20%E5%BD%93%E5%BD%93/buy/utf8/nospace/http%3A%2F%2Fsearch.dangdang.com%2F%3Fkey%3D%7Bquery%7D%26act%3Dinput)                 | http://search.dangdang.com/?key={query}&act=input              |
| 阿里巴巴       | [buy](https://s.1688.com/selloffer/offer_search.htm?keywords={query})                                                                                                                 | https://s.1688.com/selloffer/offer_search.htm?keywords={query} |
| 苏宁           | [buy](alfred://customsearch/Buy%20%22%7Bquery%7D%22%20on%20%E8%8B%8F%E5%AE%81/buy/utf8/nospace/https%3A%2F%2Fsearch.suning.com%2F%7Bquery%7D%2F)                                      | https://search.suning.com/{query}/                             |
| Amazon         | [buy](alfred://customsearch/Buy%20%22%7Bquery%7D%22%20on%20Amazon/buy/utf8/nospace/https%3A%2F%2Fwww.amazon.com%2Fs%3Fk%3D%7Bquery%7D)                                                | https://www.amazon.com/s?k={query}                             |
| Amazon(海外购) | [buy](alfred://customsearch/Buy%20%22%7Bquery%7D%22%20on%20%E4%BA%9A%E9%A9%AC%E9%80%8A%E6%B5%B7%E5%A4%96%E8%B4%AD/buy/utf8/nospace/https%3A%2F%2Fwww.amazon.cn%2Fs%3Fk%3D%7Bquery%7D) | https://www.amazon.cn/s?k={query}                              |
| 考拉海购       | [buy](alfred://customsearch/Buy%20%22%7Bquery%7D%22%20on%20%E8%80%83%E6%8B%89%E6%B5%B7%E8%B4%AD/buy/utf8/nospace/https%3A%2F%2Fsearch.kaola.com%2Fsearch.html%3Fkey%3D%7Bquery%7D)    | https://search.kaola.com/search.html?key={query}               |
| 网易严选       | [buy](alfred://customsearch/Buy%20%22%7Bquery%7D%22%20on%20%E7%BD%91%E6%98%93%E4%B8%A5%E9%80%89/buy/utf8/nospace/http%3A%2F%2Fyou.163.com%2Fsearch%3Fkeyword%3D%7Bquery%7D)           | http://you.163.com/search?keyword={query}                      |

## 设计

|                | Alfred                                                                                                                                                                                                                                  | Url                                                            |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| 阿里巴巴矢量库 | [icon](alfred://customsearch/Search%20%E9%98%BF%E9%87%8C%E5%B7%B4%E5%B7%B4%E7%9F%A2%E9%87%8F%E5%BA%93%20for%20%27%7Bquery%7D%27/icon/utf8/nospace/https%3A%2F%2Fwww.iconfont.cn%2Fsearch%2Findex%3FsearchType%3Dicon%26q%3D%7Bquery%7D) | https://www.iconfont.cn/search/index?searchType=icon&q={query} |
| easyicon       | [icon](alfred://customsearch/Search%20easyicon%20for%20%27%7Bquery%7D%27/icon/utf8/nospace/https%3A%2F%2Fwww.easyicon.net%2Flanguage.en%2Ficonsearch%2F%7Bquery%7D)                                                                     | https://www.easyicon.net/language.en/iconsearch/{query}        |
| 千图网         | icon                                                                                                                                                                                                                                    | https://588ku.com/                                             |
| Google Image   | [image](alfred://customsearch/Search%20google%20for%20%27%7Bquery%7D%27/image/utf8/nospace/https%3A%2F%2Fwww.google.com%2Fsearch%3Fq%3D%7Bquery%7D%26tbm%3Disch)                                                                        | https://www.google.com/search?q={query}&tbm=isch               |
| unsplash Image | [image](alfred://customsearch/Search%20unsplash%20for%20%27%7Bquery%7D%27/image/utf8/nospace/https%3A%2F%2Funsplash.com%2Fsearch%2Fphotos%2F%7Bquery%7D)                                                                                | https://unsplash.com/search/photos/{query}                     |
| 站长之家       | [template](alfred://customsearch/Search%20%E7%AB%99%E9%95%BF%E4%B9%8B%E5%AE%B6%20for%20%27%7Bquery%7D%27/template/utf8/nospace/http%3A%2F%2Faspx.sc.chinaz.com%2Fquery.aspx%3Fkeyword%3D%7Bquery%7D)                                    | http://aspx.sc.chinaz.com/query.aspx?keyword={query}           |

## 包搜索

|                     | Alfred                                                                                                                                                                                          | Url                                                                  |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| Docker 镜像         | [docker](alfred://customsearch/Search%20hub.docker.com%20for%20Image%20%27%7Bquery%7D%27/docker/utf8/nospace/https%3A%2F%2Fhub.docker.com%2Fsearch%3Fq%3D%7Bquery%7D%26type%3Dimage)            | https://hub.docker.com/search?q={query}&type=image                   |
| Npm 包              | [npm](alfred://customsearch/Search%20npm%20for%20package%20%27%7Bquery%7D%27/npm/utf8/nospace/https%3A%2F%2Fwww.npmjs.com%2Fsearch%3Fq%3D%7Bquery%7D)                                           | https://www.npmjs.com/search?q={query}                               |
| Composer 包         | [composer](alfred://customsearch/Search%20PHP%20package%20%27%7Bquery%7D%27/composer/utf8/nospace/https%3A%2F%2Fpackagist.org%2Fsearch%2F%3Fsearch_query%255Bquery%255D%3D%7Bquery%7D)          | https://packagist.org/search/?search_query%5Bquery%5D={query}        |
| Python 包           | [pip](alfred://customsearch/Search%20PyPI%20for%20python%20package/pip/utf8/nospace/https%3A%2F%2Fpypi.org%2Fsearch%2F%3Fq%3D%7Bquery%7D)                                                       | https://pypi.org/search/?q={query}                                   |
| Linux deb/rpm       | [apt](alfred://customsearch/Search%20Linux%20Package%20%27%7Bquery%7D%27/apt/utf8/nospace/https%3A%2F%2Fpkgs.org%2Fsearch%2F%3Fq%3D%7Bquery%7D)                                                 | https://pkgs.org/search/?q={query}                                   |
| Google 插件         | [chrome](alfred://customsearch/Search%20chrome%20plugin%20for%20%27%7Bquery%7D%27/plugin/utf8/nospace/https%3A%2F%2Fchrome.google.com%2Fwebstore%2Fsearch%2F%7Bquery%7D%3Fhl%3Dzh-CN)           | https://chrome.google.com/webstore/search/{query}?hl=zh-CN           |
| stylish             | [stylish](talfred://customsearch/Search%20userstyles%20for%20%27%7Bquery%7D%27/stylish/utf8/nospace/https%3A%2F%2Fuserstyles.org%2Fstyles%2Fbrowse%3Fsearch_terms%3D%7Bquery%7D%26type%3Dfalse) | https://userstyles.org/styles/browse?search_terms={query}&type=false |
| Greasy Fork（油猴） | [greasy](alfred://customsearch/Search%20Greasy%20Fork%20for%20%27%7Bquery%7D%27/greasy/utf8/nospace/https%3A%2F%2Fgreasyfork.org%2Fzh-CN%2Fscripts%3Futf8%3D%25E2%259C%2593%26q%3D%7Bquery%7D)  | https://greasyfork.org/zh-CN/scripts?utf8=%E2%9C%93&q={query}        |

## MACOS 软件体验

|         | Alfred                                                                                                                                            | Url                                   |
| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| Xclient | [app](alfred://customsearch/Search%20Xclient%20for%20%27%7Bquery%7D%27/app/utf8/nospace/https%3A%2F%2Fxclient.info%2Fsearch%2Fs%2F%7Bquery%7D)    | https://xclient.info/search/s/{query} |
| orsoon  | [app](alfred://customsearch/Search%20orsoon.com%20for%20%27%7Bquery%7D%27/app/utf8/nospace/https%3A%2F%2Fs.orsoon.com%2Fsearch%3Fk%3D%7Bquery%7D) | https://s.orsoon.com/search?k={query} |

## 域名

|           | Alfred                                                                                                                                                                                                          | Url                                                                                 |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| whois     | [domain](alfred://customsearch/whois%20%27%7Bquery%7D%27/domain/utf8/nospace/http%3A%2F%2Fwhois.chinaz.com%2F%7Bquery%7D)                                                                                       | http://whois.chinaz.com/{query}                                                     |
| Alicloud  | [domain](alfred://customsearch/Buy%20domain%20%27%7Bquery%7D%27%20on%20AliCloud/domain/utf8/nospace/https%3A%2F%2Fwww.alibabacloud.com%2Ftc%2Fdomain%2Fsearch%3Fkeyword%3D%7Bquery%7D)                          | https://www.alibabacloud.com/tc/domain/search?keyword={query}                       |
| Godaddy   | [domain](alfred://customsearch/Buy%20domain%20%27%7Bquery%7D%27%20on%20Goddy/domain/utf8/nospace/https%3A%2F%2Fsg.godaddy.com%2Fdomainsearch%2Ffind%3FcheckAvail%3D1%26tmskey%3D%26domainToCheck%3D%7Bquery%7D) | https://sg.godaddy.com/domainsearch/find?checkAvail=1&tmskey=&domainToCheck={query} |
| Namecheap | [domain](alfred://customsearch/Buy%20domain%20%27%7Bquery%7D%27%20on%20namecheap/domain/utf8/nospace/https%3A%2F%2Fwww.namecheap.com%2Fdomains%2Fregistration%2Fresults.aspx%3Fdomain%3D%7Bquery%7D)            | https://www.namecheap.com/domains/registration/results.aspx?domain={query}          |

## 代码/项目

|        | Alfred                                                                                                                                               | Url                                 |
| ------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------- |
| Github | [code](alfred://customsearch/Search%20Github%20for%20code%20%27%7Bquery%7D%27/code/utf8/nospace/https%3A%2F%2Fgithub.com%2Fsearch%3Fq%3D%7Bquery%7D) | https://github.com/search?q={query} |

## 其它

|                  | Alfred                                                                                                                                                                                                                        | Url                                                                                               |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| 国标             | [gb](alfred://customsearch/Search%20%E5%9B%BD%E6%A0%87%20%27%7Bquery%7D%27/gb/utf8/nospace/http%3A%2F%2Fopenstd.samr.gov.cn%2Fbzgk%2Fgb%2Fstd_list%3Fp.p1%3D0%26p.p90%3Dcirculation_date%26p.p91%3Ddesc%26p.p2%3D%7Bquery%7D) | http://openstd.samr.gov.cn/bzgk/gb/std_list?p.p1=0&p.p90=circulation_date&p.p91=desc&p.p2={query} |
| Github           | [code]()                                                                                                                                                                                                                      | https://github.com/search?q={query}                                                               |
| 天眼查（查人）   | [tyc](alfred://customsearch/Search%20%E5%A4%A9%E7%9C%BC%E6%9F%A5%20for%20People%20%27%7Bquery%7D%27/tyc/utf8/nospace/https%3A%2F%2Fwww.tianyancha.com%2Fhumansearch%2F%7Bquery%7D)                                            | https://www.tianyancha.com/humansearch/{query}                                                    |
| 天眼查（查公司） | [tyc](alfred://customsearch/Search%20%E5%A4%A9%E7%9C%BC%E6%9F%A5%20for%20Company%20%27%7Bquery%7D%27/tyc/utf8/nospace/https%3A%2F%2Fwww.tianyancha.com%2Fsearch%3Fkey%3D%7Bquery%7D)                                          | https://www.tianyancha.com/search?key={query}                                                     |
| 英语缩写查询     | [abbr](alfred://customsearch/Search%20the%20definition%20for%20Acronym%20%27%7Bquery%7D%27/abbr/utf8/nospace/https%3A%2F%2Fwww.acronymfinder.com%2F%7Bquery%7D.html)                                                          | https://www.acronymfinder.com/{query}.html                                                        |
| OEIS 查询        | [oeis](alfred://customsearch/Search%20OEIS%20for%20%27%7Bquery%7D%27/oeis/utf8/nospace/http%3A%2F%2Foeis.org%2Fsearch%3Fq%3D%7Bquery%7D)                                                                                      | http://oeis.org/search?q={query}                                                                  |

## 不支持 PC 搜索的网站

- 闲鱼

# Alfred Workflow 支持 POST Request 网页

仿照已有的 Workflow ，根据提示可以建立新的网页

导入 Workflow 后，需要修改使用的默认浏览器类型（默认为 Chrome）。同时，要在 Safari/Chrome 的 Develop 菜单中勾选 Allow Javascript from Apple Events。

如果网速不好，可以试着调节 Workflow 中等待时间。
