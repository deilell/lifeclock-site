# 人生计时 · LifeClock 官网

Android 应用「人生计时」的静态官网与下载页。纯静态、零外部依赖（无 CDN、无字体外链），可直接托管在 GitHub Pages / Cloudflare Pages / 任意静态空间。

## 结构

```
index.html              单页官网（内联 CSS/JS，图标为内联 SVG mask）
download/LifeClock.apk  当前发布版安装包，固定文件名，换版本直接覆盖
.github/workflows/       GitHub Pages 自动部署
```

## 下载链接

页面按钮指向同域相对路径 `download/LifeClock.apk`，绑自定义域名后走同一 CDN，比跳 `githubusercontent.com` 稳定得多。

历史版本归档在 Releases（tag 形如 `v1.1.0`，资产名 `LifeClock.apk`）。

## 发新版流程

1. 把新 APK 覆盖到 `download/LifeClock.apk`（保持文件名不变，HTML 无需改动）
2. 同步 `index.html` 里的版本号文案：`vX.Y.Z`、`<dt>版本</dt><dd>X.Y.Z</dd>`
3. 提交推送；同时可发一个 Release 归档
4. 应用包名：`com.zaka.lifeclock`

> 仓库体积会随版本累积，每版约 8.5 MB。版本多了可以定期用新仓库重建历史。
