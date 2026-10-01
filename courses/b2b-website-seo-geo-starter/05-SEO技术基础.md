# 05｜SEO 技术基础

## 一、理解 Google 的几个阶段

```text
已发布 → 已发现 → 已抓取 → 已索引 → 获得展示 → 点击 → 询盘
```

前一步不保证后一步。网站上线、sitemap 成功和 Search Console 请求收录都不能保证页面被索引或排名。

## 二、每个重点页面的基础检查

- URL 稳定、能表达主题；
- 独立且准确的 `<title>`；
- 简洁的 meta description；
- 一个清晰的页面主标题；
- H2/H3 帮助读者阅读，而不是机械塞词；
- 自引用 canonical 指向正式 HTTPS URL；
- robots 与页面策略一致；
- 图片文件合理、ALT 描述图片在此处的作用；
- 正文能回答搜索意图；
- 有上下文内链和明确 CTA；
- 可见内容与结构化数据一致。

Google 不使用 meta keywords。也没有神奇字数；重点是内容是否独特、可靠、易读、更新及时并真正帮助用户。

## 三、robots、noindex、canonical、redirect 的区别

| 工具 | 作用 | 不要怎么用 |
| --- | --- | --- |
| robots.txt | 管理爬虫访问路径 | 不用它代替删除索引 |
| noindex | 告诉搜索引擎不要索引页面 | 页面必须可被读取才容易看到指令 |
| canonical | 声明首选 URL | 不用它掩盖完全不同的页面 |
| 301/308 | 将旧 URL 永久迁移到新 URL | 不建立多层跳转链 |

模板化、参数不足的型号页可以先允许用户访问但 noindex；重点类别和采购指南做好后再讨论扩大索引。构建路由数量不等于 SEO 页面数量。

## 四、sitemap

- 只包含规范、希望索引、返回 200 的 URL；
- 不放重定向、404、noindex 和重复 URL；
- `lastmod` 只在页面实质更新时改变；
- 提交成功只表示 Google 能读取文件，不保证其中 URL 被抓取或索引。

## 五、Search Console 诊断顺序

1. 看报告数据截止日期；
2. 选择一个具体 URL；
3. 检查线上状态、robots、noindex、canonical 和重定向；
4. 看 Google 选择的规范页与最近抓取；
5. 检查该页是否有实质内容和内部链接；
6. 修复真实问题后再请求验证；
7. 给抓取和数据更新留时间。

“页面会自动重定向”可能是正确迁移；“已发现未索引”也不等于 DNS 或服务器故障。不要把正常状态当 bug 反复改站。

## 六、性能

先找瓶颈再优化：图片尺寸与格式、字体、关键资源、缓存、第三方脚本、服务器响应。分别检查实验室测试和真实用户数据；真实用户数据不足时不能宣布 Core Web Vitals 已通过。

## 官方资料

- https://developers.google.com/search/docs/fundamentals/seo-starter-guide
- https://developers.google.com/search/docs/crawling-indexing/sitemaps/overview
- https://support.google.com/webmasters/answer/9128668
- https://web.dev/articles/vitals
