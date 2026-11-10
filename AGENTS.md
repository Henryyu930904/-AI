# 專案名稱：統計機器學習筆記網站 (ML & Stat Notes)

## 1. 專案目的
這是一個用於整理個人統計學與機器學習筆記的靜態網站。設計目標是極簡、易讀，並能清楚展示數學公式與 Python/R 程式碼。

## 2. 檔案結構與命名規則
- 首頁固定為 `index.html`。
- 所有共用樣式統一寫在 `style.css`。
- 新增的筆記頁面必須放在 `/notes/` 資料夾下。
- 筆記檔案命名規則：全小寫英文，單字間以連字號分隔，例如 `random-forest.html`、`pca-analysis.html`。

## 3. 網頁風格與排版指南
- **顏色配置**：背景使用淺灰白 (`#f8f9fa`)，主要文字為深灰 (`#333333`)，標題與強調文字使用深藍色 (`#2c3e50`)。
- **字體**：中文優先使用微軟正黑體，英文使用 Roboto 或 Arial。程式碼區塊必須使用等寬字體 (Monospace) 並加上淺色背景。

## 4. AI 新增頁面時的標準作業流程 (SOP)
當我要求「新增一篇關於 [某主題] 的筆記」時，請嚴格遵守以下 HTML 結構模板產出檔案：

```html
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[填入筆記標題] - 統計學習筆記</title>
    <link rel="stylesheet" href="../style.css">
</head>
<body>
    <header>
        <h1>[填入筆記標題]</h1>
        <a href="../index.html">← 回到首頁</a>
    </header>
    <main>
        <section class="concept">
            <h2>核心概念</h2>
            <p>[填入演算法或統計理論的白話文解釋]</p>
        </section>
        <section class="code-example">
            <h2>實作範例</h2>
            <pre><code>[填入 Python 或 R 的重點實作程式碼]</code></pre>
        </section>
    </main>
</body>
</html>
