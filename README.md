# DENGPAN 官网（www.dengpantrade.com）

福建龙岩登攀贸易有限公司官方网站。纯静态站点（HTML/CSS/JS 单文件内联），无构建步骤。

## 线上环境

| 项目 | 值 |
|---|---|
| 正式地址 | https://www.dengpantrade.com |
| 托管 | Netlify（项目名 `dengpantrade`） |
| 备用地址 | https://dengpantrade.netlify.app |
| 域名解析 | 网易企业邮「域名解析」→ 高级解析（NS 为 ns1/ns2.myhostadmin.net） |
| 证书 | Let's Encrypt，自动续签 |

## 文件说明

| 文件 | 用途 |
|---|---|
| `index.html` | 首页 |
| `products.html` | 产品列表（分类筛选 + 产品卡片） |
| `about.html` | 公司介绍（渠道伙伴定位） |
| `contact.html` | 联系页（表单走 `mailto:`，无后端） |
| `404.html` | 404 页 |
| `_headers` | Netlify 安全响应头与缓存策略配置 |
| `robots.txt` | 爬虫规则 |
| `sitemap.xml` | 站点地图（改页面后需同步更新） |
| `og-image.png` | 社交分享缩略图 1200×630 |

## 重要约定

1. **域名解析只有 Elvis 能碰。** 竹邮面板里 4 条邮箱记录（2 条 MX + SPF + DMARC）和 1 条 DKIM 一条都不能删改，删了企业邮箱立刻收不到信。
2. **改完必须验证邮箱还活着。** 发一封测试邮件到 `elvis@dengpantrade.com`。
3. **产品配图放 `images/` 目录**，命名用小写英文加连字符，例如 `roots-blower-bk5006.jpg`。
4. **ESP（电除尘）板块已下线**，代码以注释形式保留在 `products.html` / `index.html` 中。恢复时取消注释即可，但需同步恢复 index.html 的首页卡片和页脚链接。
5. 改完 `sitemap.xml` 里的 `lastmod` 日期。

## 本地预览

直接双击 `index.html` 即可，或起一个本地服务：

```bash
python -m http.server 8765
```

## 运维记录

- 2026-10-29：网站运维由 Elvis 交接至 lian-JQ（GitHub @lian-JQ）。首次推送链路验证：本地 → GitHub → Netlify 自动部署。

## 联系方式（页面统一口径）

- 邮箱：elvis@dengpantrade.com
- 电话：+86 186 0597 0698
