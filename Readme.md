# 各网站搜索链接

为了方便直接进行搜索（而不用二次跳转），给出各网站搜索链接

有 {query} 的 Url 为 GET Request，直接将 {query} 换为需要搜索的内容即可（一般中英文都可）。Alfred 链接为 Alfred web search share link。

无 {query} 的 Url 不支持 GET Request，需要打开网页后在表单处填写。Alfred workflow 文件夹中提供了 Alfred Workflow 通过 Javascript 模拟打开。

|                | Alfred       | Url                                                                                                                |
| -------------- | ------------ | ------------------------------------------------------------------------------------------------------------------ |
| 京东           | [buy]()      | https://search.jd.com/Search?keyword={query}&enc=utf-8                                                             |
| 淘宝           | [buy]()      | https://s.taobao.com/search?q={query}                                                                              |
| 当当           | [buy]()      | http://search.dangdang.com/?key={query}&act=input                                                                  |
| 阿里巴巴       | [buy]()      | https://s.1688.com/selloffer/offer_search.htm?keywords={query}                                                     |
| 苏宁           | [buy]()      | https://search.suning.com/{query}/                                                                                 |
| Amazon         | [buy]()      | https://www.amazon.com/s?k={query}                                                                                 |
| Amazon(海外购) | [buy]()      | https://www.amazon.cn/s?k={query}                                                                                  |
| Sci-hub        | [doi]()      | https://sci-hub.se/{query}                                                                                         |
| dx.doi.org     | [doi]()      | http://dx.doi.org/{query}                                                                                          |
| Google Scholar | [essay]()    | https://scholar.google.com/scholar?q={query}                                                                       |
| 谷歌镜像       | [essay]()    | https://s3.sci-hub.org.cn//scholar?q={query}                                                                       |
| 谷歌镜像       | [essay]()    | https://xueshu.123admin.com/scholar?q={query}                                                                      |
| CNKI           | [essay]()    | http://scholar.cnki.net/result.aspx?q={query}                                                                      |
| 维普           | [essay]()    | http://www.cqvip.com/main/search.aspx?k={query}                                                                    |
| whois          | [domain]()   | http://whois.chinaz.com/{query}                                                                                    |
| Alicloud       | [domain]()   | https://www.alibabacloud.com/tc/domain/search?keyword={query}                                                      |
| Godaddy        | [domain]()   | https://sg.godaddy.com/domainsearch/find?checkAvail=1&tmskey=&domainToCheck={query}                                |
| Namecheap      | [domain]()   | https://www.namecheap.com/domains/registration/results.aspx?domain={query}                                         |
| 英语缩写查询   | [abbr]()     | https://www.acronymfinder.com/{query}.html                                                                         |
| OEIS 查询      | [oeis]()     | http://oeis.org/search?q={query}                                                                                   |
| Docker 镜像    | [docker]()   | https://hub.docker.com/search?q={query}&type=image                                                                 |
| Npm 包         | [npm]()      | https://www.npmjs.com/search?q={query}                                                                             |
| Composer 包    | [composer]() | https://packagist.org/search/?search_query%5Bquery%5D={query}                                                      |
| Python 包      | [pip]()      | https://pypi.org/search/?q={query}                                                                                 |
| Linux deb/rpm  | [apt]()      | https://pkgs.org/search/?q={query}                                                                                 |
| Genesis 书库   | [book]()     | http://gen.lib.rus.ec/search.php?req={query}&open=0&res=25&view=simple&phrase=1&column=def                         |
| 全国图书馆     | [book]()     | http://book.ucdrs.superlib.net/search?sw=%E7%AE%97%E6%B3%95%E5%AF%BC%E8%AE%BA&ecode=utf-8&channel=search&Field=all |
| 豆瓣读书       | [book]()     | https://search.douban.com/book/subject_search?search_text={query}                                                  |

## 使用 Alfred Workflow 注意事项

导入 Workflow 后，需要修改使用的默认浏览器类型（默认为 Chrome）。同时，要在 Safari/Chrome 的 Develop 菜单中勾选 Allow Javascript from Apple Events。

如果网速不好，可以试着调节 Workflow 中等待时间。

## 不支持 PC 搜索的网站

- 闲鱼
