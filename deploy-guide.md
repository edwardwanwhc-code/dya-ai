# GitHub Pages 部署指南

## 前置需求
- 一個 GitHub 帳號
- Git 已安裝（或直接用 GitHub 網頁界面）

---

## 部署步驟

### 方法一：GitHub 網頁界面（最簡單，推薦新手）

1. 登入 [github.com](https://github.com)
2. 點 **"New repository"**（右上角 + 號）
3. Repository name 填入：`dya-ai`（或你喜歡的名字）
4. 設定為 **Public**
5. 點 **"Create repository"**
6. 在新建的 repo 頁面，點 **"uploading an existing file"**
7. 將 `index.html` 和 `README.md` 拖曳上傳
8. Commit message 填 `Initial commit - DYA_AI website`
9. 點 **"Commit changes"**

### 啟用 GitHub Pages

1. 進入 repo 頁面，點頂部 **Settings**
2. 左側滾動到 **Pages**
3. Source 選 **"Deploy from a branch"**
4. Branch 選 **main**，folder 選 **/ (root)**
5. 點 **Save**

⏱️ 等待約 1-3 分鐘後，你的網址就會是：
```
https://edwardwanwhc-code.github.io/dya-ai/
```

---

### 方法二：Git 命令列（快速，適合有 Git 基礎的人）

```bash
cd "C:\Users\edwar\OneDrive\桌面\DYA_AI"

git init
git add .
git commit -m "Initial commit - DYA_AI website"

# 在 GitHub 建好 repo 後：
git remote add origin https://github.com/edwardwanwhc-code/dya-ai.git
git branch -M main
git push -u origin main
```

然後同樣在 GitHub Settings > Pages 啟用即可。

---

## 每週更新流程

```bash
# 1. 編輯 index.html（更新 Part 2 新聞內容）
# 2. 提交更改
git add index.html
git commit -m "Week XX - AI 資訊更新 (2026-XX-XX)"
git push

# GitHub Pages 會自動重新部署，通常 1-2 分鐘生效
```

---

## 你的最終網址

```
https://edwardwanwhc-code.github.io/dya-ai/
```

將此網址放入 IG Bio Link 即可！
