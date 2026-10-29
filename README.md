# 人生计时 · LifeClock 官网

Android 应用「人生计时」的静态官网与下载页。

- 站点：`index.html`（纯静态，零依赖，仅通过 jsDelivr 加载 remixicon 图标字体）
- 下载：APK 发布在本仓库 Releases，资产名固定为 `LifeClock.apk`，页面使用
  `https://github.com/deilell/lifeclock-site/releases/latest/download/LifeClock.apk`
  这个永久链接，因此换版本时**不需要改 HTML**，只要发布新 Release 并沿用同名资产。
- 应用包名：`com.zaka.lifeclock`

## 发新版流程

1. 新建 Release，tag 形如 `v1.1.0`
2. 上传 APK，资产名**必须**为 `LifeClock.apk`
3. 如需同步页面文案，改 `index.html` 里的版本号（`v1.1.0` / `<dd>版本</dd>`）后提交
