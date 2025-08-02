# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 專案概述

這是一個使用 Slidev 框架建立的簡報專案，用於在 NCHC (National Center for High-performance Computing) 進行 CDX 使用經驗分享。內容為繁體中文簡報，聚焦於 CDX 平台的使用經驗與心得分享。

## 開發指令

### 環境設定與開發
- `npm install` - 安裝專案依賴套件
- `npm run dev` - 啟動開發伺服器（預設開啟 http://localhost:3030）
- `slidev --open slides.mdc` - 直接使用 Slidev 指令啟動

### 建置與匯出
- `npm run build` - 建置生產版本
- `npm run export` - 匯出簡報（例如：PDF 格式）

## 專案架構與結構

### 核心檔案
- `slides.mdc` - 主要簡報內容，使用 Markdown 格式搭配 Slidev 語法
- `components/CustomToc.vue` - 自訂目錄 Vue 元件，可依版面類型篩選投影片
- `snippets/external.ts` - 簡報中使用的 TypeScript 程式碼片段
- `public/` - 靜態資源資料夾，包含簡報使用的圖片

### 主題與設定
- 使用自訂 Slidev 主題：`@cxphoenix/slidev-theme-fhsh-aisp`
- 設定 slide-left 轉場效果
- 封面頁不顯示頁碼
- 繁體中文內容，專注於 CDX 平台使用經驗分享

### 部署設定
- GitHub Actions 自動部署至 GitHub Pages（當 main 分支有推送時）
- 同時支援 Netlify 和 Vercel 部署
- 使用 Node.js LTS 版本

### 元件結構
`CustomToc` 元件的篩選功能：
- 依版面類型篩選（section、default、image）
- 支援頁面範圍設定
- 排除封面頁不顯示在目錄中

編輯簡報時請維持既有的 Slidev 語法和版面結構。本簡報採用結構化格式，包含章節、圖片和自訂元件。

## 文件撰寫準則

### 語言使用
- 撰寫 README 或 git commit 內容時，必須使用台灣慣用繁體中文用語
- 專業術語保持英文書寫（如：CDX、Slidev、GitHub Actions）
- 適當使用 emoji 增加文件的趣味性和可讀性 ✨

### 編輯注意事項
- 維持 Slidev 語法的一致性
- 保持簡報內容的結構化格式
- 圖片資源放置於 `public/` 資料夾中

## Git 提交指令

### 提交訊息特殊處理
- git commit message 直接在 stdout 輸出，不用幫我進行 git commit