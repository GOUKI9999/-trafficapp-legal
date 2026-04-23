# Red Green Light · Legal pages

Google Play legal pages for the Android app
**Red Green Light** (`com.gouki9999.trafficlight`).

Hosted via GitHub Pages.

## 文件

| File | Purpose |
|------|---------|
| `index.html` | Landing page with links to the two legal docs |
| `privacy-policy.html` | Privacy policy (EN + 中) |
| `terms-of-service.html` | Terms of service (EN + 中) |
| `style.css` | Shared styles |

## 如何部署到 GitHub Pages

1. 新建一个**公开**仓库,名字随意(比如 `trafficapp-legal`)
2. 把本目录里的所有文件推到该仓库 root:
   ```bash
   git init
   git add .
   git commit -m "legal pages"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo>.git
   git push -u origin main
   ```
3. 仓库 **Settings → Pages**:
   - Source: `Deploy from a branch`
   - Branch: `main` · Folder: `/ (root)`
   - Save
4. 等 1-2 分钟,页面会发布在:
   ```
   https://<your-username>.github.io/<repo>/
   ```
5. 测试三个链接都打得开:
   - `/` → index
   - `/privacy-policy.html`
   - `/terms-of-service.html`

## 填到 Play Console

- **Privacy policy URL**:
  `https://<your-username>.github.io/<repo>/privacy-policy.html`
- 服务条款 URL 不是必填项,但可以在 listing 的详细描述末尾加一句:
  "Terms: https://<your-username>.github.io/<repo>/terms-of-service.html"

## 后续修改

只要你 push 新 commit 到 main 分支,GitHub Pages 自动重新部署
(约 1 分钟)。两个 html 页脚的日期需要和实际发布同步。
