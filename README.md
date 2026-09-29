# 我的 Codex B2B 增长技能库

这是一套从真实建站、SEO/GEO、Facebook 运营、主动开发和视频生产工作中提炼出来的可安装 Codex Skills。仓库只保留可复用的方法、门槛、模板和验收规则；客户名单、账号、邮箱、电话、询盘正文、发送记录和密钥均不进入公开仓库。

## 技能目录

| 分类 | 技能 | 解决的问题 |
| --- | --- | --- |
| 建站 | `wordpress-b2b-site-ops` | 规划并交付以询盘为目标的 WordPress B2B 网站 |
| SEO/GEO | `b2b-seo-geo-ops` | 关键词研究、页面归属、内容、内链、结构化数据与复盘 |
| 建站性能 | `wordpress-performance-qa` | 在不破坏表单、统计和页面功能的前提下优化性能 |
| 询盘 | `b2b-inquiry-response-ops` | 新询盘、老客户待回复、七天未回复跟进的分阶段运营 |
| Facebook | `facebook-b2b-content-ops` | 把工厂证据转成买家愿意看的内容并持续复盘 |
| Facebook 广告 | `facebook-lead-ads-ops` | 用受众、创意和高意向表单筛选合格线索 |
| Facebook 主动开发 | `facebook-b2b-prospecting` | 从公开主页发现、核验、评分和去重潜在买家 |
| Google Maps | `google-maps-b2b-prospecting` | 用窄搜索词和多源验证建立地图买家短名单 |
| TikTok | `tiktok-b2b-buyer-discovery` | 把补货、上新等内容信号验证成真实 B2B 买家 |
| 外联实验 | `b2b-outreach-experiments` | 用 15 人小批量、单变量测试和停损门槛迭代外联 |
| 视频策划 | `b2b-video-material-to-script` | 完整审片、证据分级、选段和生成可执行剪辑脚本 |
| HyperFrames | `hyperframes-b2b-video-production` | 以确定性时间轴制作并验证 B2B 竖屏视频 |
| AI 视频 | `ai-video-prompt-workflow` | 用角色/产品一致性与因果连续性设计分镜提示词 |

更详细的分类、边界和组合方式见 [docs/CATALOG.md](docs/CATALOG.md)。来源覆盖和脱敏原则见 [docs/SOURCE-COVERAGE.md](docs/SOURCE-COVERAGE.md) 与 [docs/SECURITY-AND-PRIVACY.md](docs/SECURITY-AND-PRIVACY.md)。

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
