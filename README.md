# Dongshuo Zhang — Minimal Light 学术主页

这是从 `alandszhang/alandszhang.github.io` 迁移的完整 Jekyll 源码，基于 [Minimal Light](https://github.com/yaoyao-liu/minimal-light)，保留原站头像、介绍、10 条 News、2 篇论文详情、2 场报告、Google Scholar、GitHub 和邮箱。

## 修改内容

| 文件 | 用途 |
| --- | --- |
| `_config.yml` | 姓名、职位、单位、邮箱、头像和学术链接 |
| `index.md` | 个人介绍和研究方向 |
| `_data/news.yml` | 新闻动态，按时间倒序排列；前 5 条直接显示，其余可展开 |
| `_publications/*.md` | 每篇论文的元数据与详情正文 |
| `_talks/*.md` | 报告信息与正文 |
| `cv.md` | 在线 CV，根据原站真实经历整理 |
| `assets/css/style.scss` | 个性化排版、颜色、手机和深色模式 |
| `assets/img/avatar.png` | 原站头像 |

新增论文时，复制 `_publications` 中的一篇并修改 `title`、`date`、`authors`、`venue`、`venue_short`、`permalink`。`paperurl`、`code`、`project` 都是可选项，不要填写空链接。独立的 Publications 页面会自动按日期倒序更新；首页不显示 Selected Publications。

## 本地运行

使用 Ruby 3.1 或兼容的 Ruby 环境：

```sh
bundle install
bundle exec jekyll serve --host 127.0.0.1
```

访问终端显示的本地网址。无需 npm、远程主题或 Google Fonts。

## 应用到现有 GitHub Pages

1. 先给旧站创建备份分支，例如 `backup-before-minimal-light`。
2. 在本地克隆旧仓库，并创建迁移分支 `minimal-light-redesign`。
3. 清理迁移分支中的旧主题文件（保留 `.git`），把本目录的完整内容放到仓库根目录。请包含 `.gitignore` 等隐藏文件。
4. 提交并推送迁移分支，在 GitHub 创建 Pull Request，确认内容后合并。
5. 对使用 GitHub 原生 Jekyll 构建的仓库，在 **Settings → Pages → Build and deployment** 选择 **Deploy from a branch**、`master`、`/(root)`。如仓库使用自定义 Actions 工作流，请先确认它构建仓库根目录中的 Jekyll 源码。

不要只覆盖 `_config.yml` 后保留全部旧主题：旧布局、示例文章和集合会干扰新站。不要把预览用的 `_site` 目录作为源码上传。

原域名继续是 https://alandszhang.github.io/ ，无需购买域名。

## 需要你以后补充的内容

- 原站没有真实 CV PDF。现提供在线 CV；准备好 PDF 后，将其放到 `assets/files/cv.pdf`，并启用 `_config.yml` 中的 `cv_pdf`。
- DriftAD、IROS 2026、Motion-Feat 和 SHAA 的信息先保留在 News；未补造原站缺失的完整论文元数据。
- 原论文没有配图，因此当前论文列表采用文字排版，未使用其他研究人员的示例图片。

详细迁移记录见 `MIGRATION.md`。模板源码的 CC0 文本在 `LICENSE-MINIMAL-LIGHT`，原 Academic Pages 的 MIT 声明在 `LICENSE-ACADEMICPAGES`；个人内容保持原有权利归属。
