# 技能分类与组合方式

## 一、建站、SEO 与 GEO

- 环境与资料：`environment-awareness`、`document-processor`、`tavily-search`、`find-skills`、`b2b-global-data-platform`。
- 架构与页面：`b2b-website-architecture`、`wordpress-b2b-site-ops`、`b2b-content-marketing`、`b2b-lead-generation`。
- SEO/GEO 与转化：`seo-expert`、`b2b-seo-geo-ops`、`cro-expert`。
- 视觉与性能：`b2b-visual-assets-generator`、`og-image-skill`、`image-optimizer`、`wordpress-performance-qa`。
- 验收与改进：`agent-browser`、`visual-qa`、`error-experience-learner`。

推荐顺序：环境和资料检查 → 买家路径与网站架构 → 页面和内容 → SEO/GEO 与询盘转化 → 图片和性能 → 浏览器与视觉验收 → 复盘错误。

完整技能说明、具体路径和常用组合见 [`docs/WEBSITE-BUILDING-SKILL-PACK.md`](WEBSITE-BUILDING-SKILL-PACK.md)。

零基础学习路径见 [`courses/b2b-website-seo-geo-starter`](../courses/b2b-website-seo-geo-starter/README.md)。教程解释为什么和如何做；技能提供给 Codex 执行。

## 二、询盘与客户沟通

- `b2b-inquiry-response-ops`：严格按“新询盘 → 老客户待回复 → 七天未回复”推进；每封先出稿、批准后发送、发送后验证。

它是独立的收件箱运营技能，不承担陌生客户搜集。

## 三、Facebook 运营

- `facebook-b2b-content-ops`：证据型内容、栏目规划、短视频结构和业务指标复盘。
- `facebook-lead-ads-ops`：高意向表单、受众和素材单变量测试、合格线索成本。
- `facebook-b2b-prospecting`：公开主页搜寻、官网交叉验证、联系人质量、去重和评分。

内容与广告可组合使用；主动开发单独建立名单，不能把“看到主页”当作“已验证买家”。

## 四、主动开发与外联

- `google-maps-b2b-prospecting`：地点型渠道，适合按“产品 + 买家类型 + 城市”搜寻。
- `tiktok-b2b-buyer-discovery`：内容信号型渠道，适合寻找补货、上新等内容信号验证成真实 B2B 买家 |
| 外联实验 | `b2b-outreach-experiments` | 用 15 人小批量、单变量测试和停损门槛迭代外联 |
| 视频策划 | `b2b-video-material-to-script` | 完整审片、证据分级、选段和生成可执行剪辑脚本 |
| HyperFrames | `hyperframes-b2b-video-production` | 以确定性时间轴制作并验证 B2B 竖屏视频 |
| AI 视频 | `ai-video-prompt-workflow` | 用角色/产品一致性与因果连续性设计分镜提示词 |

更详细的分类、边界和组合方式见 [docs/CATALOG.md](docs/CATALOG.md)。来源覆盖和脱敏原则见 [docs/SOURCE-COVERAGE.md](docs/SOURCE-COVERAGE.md) 与 [docs/SECURITY-AND-PRIVACY.md](docs/SECURITY-AND-PRIVACY.md)。

### 建站全流程技能包

建站相关技能已按“环境与资料 → 架构与页面 → SEO/GEO 与转化 → 视觉与性能 → 上线验收与复盘”重新分类。完整清单、调用顺序和安装方式见：

- [建站全流程技能包](docs/WEBSITE-BUILDING-SKILL-PACK.md)

## 小白建站教程

如果你想从域名、Codex、GitHub、Vercel 开始，建立网站并继续做 SEO / GEO，请按顺序阅读：

- [小白外贸独立站：从建站到 SEO / GEO 运营](courses/b2b-website-seo-geo-starter/README.md)

教程与技能分开存放：`courses/` 用于学习，`skills/` 用于让 Codex 执行具体工作流。

## 安装

克隆仓库后，将需要的单个技能目录复制到 Codex 技能目录：

```powershell
git clone https://github.com/romancenanyi-png/my-codex-skills.git
Copy-Item -Recurse .\my-codex-skills\skills\facebook-b2b-content-ops "$env:USERPROFILE\.codex\skills\"
```

也可以一次复制全部技能：

```powershell
Copy-Item -Recurse .\my-codex-skills\skills\* "$env:USERPROFILE\.codex\skills\"
```

重新打开 Codex 后，直接说“使用 `$facebook-b2b-content-ops` 制定下周内容计划”即可。技能不会自动取得账号权限，也不会自动发送邮件、消息或广告；涉及发布、发送和预算时仍需明确授权。

## 使用原则

- 先提供真实业务信息，再让技能执行；未知数据必须标为未知，不能补猜。
- 研究、起草、批准、发送分开；公开联系人不等于允许自动群发。
- 所有平台都以合格询盘、回复、报价或样品机会为业务指标，而不是只看流量。
- 任何能力、认证、交期、产能和客户案例都必须有证据支持。

## 许可

代码和技能文本采用 [MIT License](LICENSE)。第三方平台、商标和服务各自受其条款约束。
