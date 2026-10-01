# 04｜GitHub、Vercel 与域名

## 一、四个角色

| 工具 | 大白话解释 |
| --- | --- |
| Codex | 在项目中读取、修改、测试代码的协作工具 |
| GitHub | 保存代码版本和变更历史的仓库 |
| Vercel | 从 GitHub 拉取代码、构建并托管网站的平台 |
| 域名 | 客户访问正式网站的门牌 |

## 二、GitHub 基本流程

```bash
git status
git add <明确的文件>
git diff --cached
git commit -m "Describe the scoped change"
git push origin main
```

小白应先理解：commit 是本地版本快照，push 才会把提交送到远程仓库。团队项目优先使用分支和 Pull Request，不要在不理解差异时直接覆盖主分支。

## 三、Vercel 发布

1. 在 Vercel 导入正确的 GitHub 仓库；
2. 确认 Framework Preset、Root Directory、Install Command、Build Command 和输出设置；
3. 添加生产需要的环境变量，但不把值写进 GitHub；
4. 触发部署；
5. 确认 Production 部署对应预期 commit；
6. 在正式 URL 检查页面、资源、表单、metadata、robots 和 sitemap。

曾使用过 Vite、Next.js 或其他框架的项目，最容易保留错误的根目录或输出目录。以当前 `package.json` 和实际构建结果为准，不根据旧提示词猜。

## 四、域名连接

1. 在 Vercel 添加根域名和 `www`；
2. 按平台给出的记录修改 DNS；
3. 选择一个主版本，例如 `https://www.example.com`；
4. 其余版本永久跳转到主版本；
5. canonical、sitemap、内部链接统一使用主版本；
6. 等待 DNS 生效并检查 HTTPS。

不要频繁切换 DNS。单次本地超时先用多个网络或权威查询核对，不能直接诊断为全球不可访问。

## 五、表单和邮箱

真实验收分三层：

1. 浏览器得到明确成功响应；
2. 表单/邮件服务接受提交；
3. 企业邮箱在收件箱或垃圾箱收到标记测试邮件。

更换收件邮箱时要检查实际端点、环境变量、前端构建时变量、服务激活状态和所有表单入口。测试邮件必须带唯一编号，不能计入真实询盘。

## 六、上线记录

```text
日期：
Commit：
Vercel Deployment：
正式域名：
变更页面：
构建/测试：
表单测试编号：
未解决风险：
回滚方式：
```

官方参考：

- https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories
- https://vercel.com/docs/git
- https://vercel.com/docs/domains
