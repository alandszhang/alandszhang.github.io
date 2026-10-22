# 迁移记录

- 原站来源： https://github.com/alandszhang/alandszhang.github.io
- 原站提交： `77ed1444f7e06f5f84353559f171d94bb72461f8`
- Minimal Light 来源： https://github.com/yaoyao-liu/minimal-light
- 模板提交： `dd114c3fef2d97adc1c6b6d46901e0d96ab83a7c`
- 迁移日期：2026-10-22

## 保留的真实内容

原头像、简介及机构/导师链接、邮箱、Google Scholar、GitHub，全部 10 条 News、2 篇论文及原 citation/PDF 链接、2 场报告和时间地点。个人介绍修正 “lead” 为过去时 “led”，并根据用户更正更新当前任职。首页拆出 Research Interests，表述来自原简介。CV 汇总既有信息和用户补充，没有使用旧 CV 的示例学位或虚构任职。

保留 Google Search Console 的验证文件 `google3cf6c799bd46d1ad.html`。

## URL 兼容

- `/`、`/publications/`、`/talks/`、`/cv/`
- `/publication/iros23_atten/`、`/publication/iros24_curricularvpr/`
- `/talks/greater_bay/`、`/talks/moratuwa/`
- `/about/`、`/about.html` 跳转到首页，`/resume/` 跳转到在线 CV。

旧论文和报告的无末尾斜杠链接，在 GitHub Pages 的目录服务下会跳转到相应目录 URL。

## 移除或替换

- Academic Pages 的默认博客、教学、portfolio、模板纸张/幻灯片 PDF、示例 CV、站点占位作者和无用配置。
- Minimal Light 的示例姓名、论文、头像、CV、模板演示域名、Google Analytics ID。
- 未引入 Google Fonts、第三方图标 CDN 或访客追踪。

## 尚待完善

原站 2026 年和部分 2025 年成果仅出现在 News 中，未提供完整论文条目。独立 Publications 页面保留原站两篇完整记录；作者使用原 citation 中的缩写，未推断姓名。当前没有论文缩略图、报告幻灯片或真实 CV PDF。

## 用户修改

- 当前已离开 Sony，回到 NTU 任 Research Fellow；同步更新 About Me、侧栏、搜索/分享描述和在线 CV。没有推断具体入职或离职日期。
- 移除首页 Selected Publications 区块和 All publications 链接，保留独立 Publications 页面及论文详情网址。
- About Me 按当前工作与研究目标、研究经历、教育背景、产业经历重写，具体研究方向集中放在 Research Interests。
- 补充 CamSense 已在港交所上市（06802.HK），并同步到 CV。上市信息来源：港交所披露页面（https://www1.hkexnews.hk/search/titlesearch.xhtml?category=0&lang=EN&market=SEHK&stockId=1000317690）及金杜参与上市项目的公告（https://www.kingandwood.com/hk/en/about-us/media-center/king-wood-advises-on-camsenses-successful-h-share-listing-on-the-main-board-of-the-hong-kong-stock-exchange.html）。
- 移除首页、导航和 CV 中的 Talks 展示，原报告网址保留兼容。

## 部署状态

此目录是 Minimal Light 迁移后的 Jekyll 源码。部署目标为 `alandszhang/alandszhang.github.io`；发布状态以 GitHub 仓库提交及 Pages 构建状态为准。

## 验证结果

- `bundle exec jekyll build` 构建通过（Jekyll 3.10.0）。
- 13 个生成的 HTML 页面的内部链接、锚点、样式及图片路径检查通过。
- 1280px 宽屏：双栏，侧栏 sticky，页面无横向溢出。
- 390px 手机：单栏，页面无横向溢出，头像正常加载。
- Earlier news 展开后显示全部 10 条新闻。
- 论文详情及引用内容浏览器检查通过；原无斜杠论文/报告路径可重定向。
- 外部论文 PDF 链接按原站迁移，未验证所有第三方网站的可用性。
