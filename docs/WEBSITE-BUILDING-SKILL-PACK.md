# 建站全流程技能包

这份索引把仓库里与建站直接相关的技能按实际工作阶段分类。下次建站时先判断当前处于哪个阶段，再调用对应技能；不需要一次加载全部技能。

## 一、推荐使用顺序

```text
环境检查与资料整理
→ 市场研究与网站架构
→ 页面实施与内容生产
→ SEO / GEO 与转化设计
→ 图片、性能和视觉验收
→ 上线复盘与错误沉淀
```

## 二、技能分类

### 1. 环境、资料与研究

| 技能 | 什么时候用 | 路径 |
| --- | --- | --- |
| `environment-awareness` | 开工前识别框架、依赖、命令、环境变量和部署目标 | [`skills/environment-awareness`](../skills/environment-awareness/) |
| `document-processor` | 把产品表、PDF、截图和旧网站资料整理成结构化内容 | [`skills/document-processor`](../skills/document-processor/) |
| `tavily-search` | 调研最新竞品、SERP、市场和技术资料；需要 Tavily 配置 | [`skills/tavily-search`](../skills/tavily-search/) |
| `find-skills` | 当前仓库能力不足时，查找并核验新的可安装技能 | [`skills/find-skills`](../skills/find-skills/) |
| `b2b-global-data-platform` | 设计客户、市场、关键词、内容和线索的统一数据结构 | [`skills/b2b-global-data-platform`](../skills/b2b-global-data-platform/) |

### 2. 网站架构、页面与内容

| 技能 | 什么时候用 | 路径 |
| --- | --- | --- |
| `b2b-website-architecture` | 写页面前规划买家路径、URL、导航、内链与询盘入口 | [`skills/b2b-website-architecture`](../skills/b2b-website-architecture/) |
| `wordpress-b2b-site-ops` | 交付以询盘为目标的 WordPress B2B 网站 | [`skills/wordpress-b2b-site-ops`](../skills/wordpress-b2b-site-ops/) |
| `b2b-content-marketing` | 规划主题集群、博客、案例、白皮书和内容日历 | [`skills/b2b-content-marketing`](../skills/b2b-content-marketing/) |
| `b2b-lead-generation` | 设计表单、线索评分、转化路径和销售交接 | [`skills/b2b-lead-generation`](../skills/b2b-lead-generation/) |

### 3. SEO、GEO 与转化率

| 技能 | 什么时候用 | 路径 |
| --- | --- | --- |
| `seo-expert` | 做技术 SEO、关键词映射、Schema、内容结构和 AI 搜索优化 | [`skills/seo-expert`](../skills/seo-expert/) |
| `b2b-seo-geo-ops` | 用真实网站运营节奏执行 SEO/GEO 并按周期复盘 | [`skills/b2b-seo-geo-ops`](../skills/b2b-seo-geo-ops/) |
| `cro-expert` | 审查首页、落地页、CTA 和表单的转化阻力 | [`skills/cro-expert`](../skills/cro-expert/) |

### 4. 视觉、分享图与图片性能

| 技能 | 什么时候用 | 路径 |
| --- | --- | --- |
| `b2b-visual-assets-generator` | 规划首页主图、产品流程图、案例图和营销视觉 | [`skills/b2b-visual-assets-generator`](../skills/b2b-visual-assets-generator/) |
| `og-image-skill` | 制作网页或文章的 Open Graph 社交分享图方案 | [`skills/og-image-skill`](../skills/og-image-skill/) |
| `image-optimizer` | 优化图片格式、尺寸、响应式加载、alt 和 LCP | [`skills/image-optimizer`](../skills/image-optimizer/) |
| `wordpress-performance-qa` | 在不破坏表单和统计的前提下做性能优化与回归 | [`skills/wordpress-performance-qa`](../skills/wordpress-performance-qa/) |

### 5. 浏览器测试、视觉验收与持续改进

| 技能 | 什么时候用 | 路径 |
| --- | --- | --- |
| `agent-browser` | 打开真实网页，测试导航、表单、移动端和页面状态 | [`skills/agent-browser`](../skills/agent-browser/) |
| `visual-qa` | 检查桌面、平板、手机端布局、可访问性和视觉回归 | [`skills/visual-qa`](../skills/visual-qa/) |
| `error-experience-learner` | 记录构建、部署和工具错误，避免下次重复踩坑 | [`skills/error-experience-learner`](../skills/error-experience-learner/) |

## 三、常用组合

### 从零规划 B2B 独立站

1. `environment-awareness`
2. `document-processor`
3. `b2b-website-architecture`
4. `b2b-content-marketing`
5. `b2b-lead-generation`
6. `seo-expert`

### 网站上线前验收

1. `agent-browser`
2. `visual-qa`
3. `image-optimizer`
4. `wordpress-performance-qa`
5. `seo-expert`

### 网站上线后持续运营

1. `b2b-seo-geo-ops`
2. `cro-expert`
3. `b2b-content-marketing`
4. `b2b-lead-generation`
5. `error-experience-learner`

## 四、安装方式

只安装一个技能：

```powershell
Copy-Item -Recurse .\my-codex-skills\skills\seo-expert "$env:USERPROFILE\.codex\skills\"
```

一次安装全部技能：

```powershell
Copy-Item -Recurse .\my-codex-skills\skills\* "$env:USERPROFILE\.codex\skills\"
```

安装后重新打开 Codex，再在任务中明确说“使用 `$技能名`”。教程内容仍放在 [`courses/b2b-website-seo-geo-starter`](../courses/b2b-website-seo-geo-starter/README.md)，技能与教程不混放。

## 五、安全边界

- 不把客户名单、联系人、询盘正文、邮箱、电话、Cookie、API 密钥或合同上传到公开仓库。
- 研究、起草、批准、发布分开；技能本身不代表已经获得上线、发送或投放权限。
- 来源不明的技能先审查说明和依赖，再决定是否安装。
- 页面内容、能力声明和案例只使用能够核验的证据，缺失信息标为 `unknown`。
