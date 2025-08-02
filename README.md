# CDX 使用經驗分享簡報 📊

![License](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)
![Slidev](https://img.shields.io/badge/Slidev-52.1.0-blue?style=flat-square&logo=slidev)
![Vue.js](https://img.shields.io/badge/Vue.js-3.5.18-4FC08D?style=flat-square&logo=vue.js)
![Node.js](https://img.shields.io/badge/Node.js-LTS-339933?style=flat-square&logo=node.js)
![Netlify](https://img.shields.io/badge/Deploy-Netlify-00C7B7?style=flat-square&logo=netlify)

> [!NOTE]
> 使用 Slidev 框架製作的 NCHC CDX 平台使用經驗分享簡報
>
> [README is powered by Claude code.](https://www.anthropic.com/claude-code)

這是一個專為 NCHC (National Center for High-performance Computing) 製作的 CDX 使用經驗分享簡報專案，內容聚焦於 CDX 平台的實際使用心得與最佳實務分享。

## 快速開始 🚀

### 環境需求
- Node.js LTS 版本
- npm 或其他套件管理工具

### 開發步驟
```bash
# 安裝依賴套件
npm install

# 啟動開發伺服器
npm run dev

# 瀏覽器將自動開啟 http://localhost:3030
```

## 專案特色 ✨

- 🎨 使用自訂 Slidev 主題：`@cxphoenix/slidev-theme-fhsh-aisp`
- 📑 自訂目錄元件 `CustomToc`，支援版面類型篩選
- 🔄 Slide-left 轉場效果
- 🌐 支援多平台自動部署（Netlify、Vercel）
- 📱 響應式設計，適配各種螢幕尺寸

## 開發指令 🛠️

```bash
# 開發模式
npm run dev

# 建置生產版本
npm run build

# 匯出簡報（PDF 等格式）
npm run export
```

## 專案架構 📁

```
├── slides.mdc              # 主要簡報內容
├── components/
│   └── CustomToc.vue       # 自訂目錄元件
├── snippets/
│   └── external.ts         # TypeScript 程式碼片段
├── public/                 # 靜態資源（圖片等）
├── package.json            # 專案設定與依賴
├── netlify.toml           # Netlify 部署設定
└── vercel.json            # Vercel 部署設定
```

### 核心檔案說明

- **slides.mdc**: 使用 Markdown 格式搭配 Slidev 語法的主要簡報內容
- **CustomToc.vue**: 可依版面類型（section、default、image）篩選投影片的自訂目錄元件
- **public/**: 包含簡報中使用的所有圖片和靜態資源

## 部署資訊 🌐

本專案支援多種部署平台：

### Netlify
- 自動偵測 `main` 分支推送
- 使用 Node.js 20 環境
- 自動建置與部署

### Vercel
- 支援一鍵部署
- 自動 HTTPS 與 CDN 加速

## 技術細節 🔧

- **框架**: [Slidev](https://sli.dev/) - 開發者友善的簡報框架
- **主題**: 自訂主題 `@cxphoenix/slidev-theme-fhsh-aisp`
- **版本**: Slidev ^52.1.0
- **語言**: 繁體中文內容

## 編輯指南 📝

- 主要內容編輯 `slides.mdc` 檔案
- 維持既有的 Slidev 語法和版面結構
- 圖片資源放置於 `public/` 資料夾
- 使用 `CustomToc` 元件建立結構化目錄

## 相關資源 📚

- [Slidev 官方文件](https://sli.dev/)
- [Slidev GitHub](https://github.com/slidevjs/slidev)
- [Vue.js 文件](https://vuejs.org/)

---

📅 **簡報日期**: 2025/08/11  
👨‍🏫 **講者**: CXPh03n1x @ FHSH  
🏢 **場合**: NCHC CDX 使用經驗分享
