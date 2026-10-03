# 我的健身计划 PWA v3

这是 v2 的 PWA 版本。

## 新增
- PWA manifest
- Service Worker
- 离线缓存
- Android/Chrome 添加到主屏幕
- 独立 App 窗口运行
- 手机竖屏优先
- App 图标

## 如何使用

### 方式一：推荐
把整个文件夹部署到 HTTPS 网站，例如 GitHub Pages、Vercel、Netlify 等。

然后用 Android Chrome 打开网站：
1. 打开网站
2. 浏览器菜单
3. 选择“添加到主屏幕”或“安装应用”
4. 安装后桌面会出现“健身计划”

### 方式二：本地开发
不能只双击 `index.html` 来完整测试 PWA，因为 Service Worker 通常需要 HTTPS 或 localhost。

本地启动：
```bash
python3 -m http.server 8080
```
然后打开：
http://localhost:8080

## 数据
训练打卡和重量数据仍保存在浏览器 localStorage 中。

## 注意
如果要让手机真正安装 PWA，必须通过 HTTPS 网站访问（localhost 开发环境除外）。
