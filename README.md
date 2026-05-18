# Humanizer-zh

> 去除文字中的 AI 生成痕跡，讓文字聽起來更自然、更像人類書寫。

## 簡介

Humanizer-zh 是一個用於去除文字中 AI 生成痕跡的工具。本專案翻譯自 [blader/humanizer](https://github.com/blader/humanizer)，並參考 [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop) 的實用工具部分。

核心規則基於維基百科的 [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)，由 WikiProject AI Cleanup 維護。

## 安裝

### 方法一：npx 一鍵安裝（推薦）

```bash
npx skills add https://github.com/chenboyo/humanizer-zh.git
```

### 方法二：手動安裝

1. 下載本專案的 ZIP 檔案或克隆到本地
2. 將 `SKILL.md` 複製到 Hermes Agent 的 skills 目錄：
   - **Windows**: `%USERPROFILE%\AppData\Local\hermes\skills\humanizer-zh\`
   - **macOS/Linux**: `~/.hermes/skills/humanizer-zh/`

## 使用方式

在對話中輸入：

```
用 humanizer 處理這篇文章：

[貼上你的文字]
```

## 偵測的 AI 痕跡模式

### 內容模式
1. 過度強調意義、遺產和更廣泛的趨勢
2. 過度強調知名度和媒體報導
3. 以 -ing 結尾的膚淺分析
4. 宣傳和廣告式語言
5. 模糊歸因和含糊措辭
6. 提綱式的「挑戰與未來展望」部分
6b. 「它告訴你……但它沒告訴你……」對比結構
6c. **假客觀中立（打平等板）** ← 新增
6d. **「我不是要你不信……」假裝客觀開場** ← 新增
6e. **列舉式結尾問題（1. 2. 3. 4.）** ← 新增
6f. **「就這麼簡單」收尾** ← 新增

### 語言和語法模式
7. 過度使用的「AI 詞彙」
8. 避免使用「是」（係動詞迴避）
9. 否定式排比
10. 三段式法則過度使用
11. 刻意換詞（同義詞循環）
12. 虛假範圍

### 風格模式
13. 破折號過度使用
13b. 冒號製造「揭露感」
13c. **「發現」開場白**（我重新看了一遍……發現……）
13d. **情緒升級結構**（更讓我覺得……的是）
13e. **「後來我做了……」段落過渡**
14. 粗體過度使用
15. 內聯標題垂直列表
16. 表情符號裝飾
17. 彎引號

### 交流模式
18. 協作交流痕跡
19. 知識截止日期免責聲明
20. 諂媚/卑躬屈膝的語氣

### 填充詞和迴避
21. 填充短語
22. 過度限定
23. 通用積極結論

## 品質評分

對改寫後的文字進行 1-10 分評估（總分 50）：

| 維度 | 評估標準 |
|------|---------|
| **直接性** | 直接陳述事實還是繞圈宣告？ |
| **節奏** | 句子長度是否變化？ |
| **信任度** | 是否尊重讀者智慧？ |
| **真實性** | 聽起來像真人說話嗎？ |
| **精煉度** | 還有可刪減的內容嗎？ |

- 45-50 分：優秀，已去除 AI 痕跡
- 35-44 分：良好，仍有改進空間
- 低於 35 分：需要重新修訂

## 與原專案的差異

本專案在原版基礎上，新增了以下規則（基於實際修改經驗）：

- **6c. 假客觀中立**：AI 習慣在結尾把所有相關方「打平等板」，假裝客觀
- **6d. 假裝客觀開場**：「我不是要你不信……」然後接結論
- **6e. 列舉式結尾**：「我會先問自己幾個問題：1. 2. 3. 4.」
- **6f. 「就這麼簡單」收尾**：暗示讀者現在已經理解了
- **13c. 「發現」開場白**：「我重新看了一遍……發現一些很有意思的東西」
- **13d. 情緒升級結構**：「更讓我覺得……的是」
- **13e. 段落過渡**：「後來我做了一個思想實驗」

## 授權

MIT License

## 參考

- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
- [blader/humanizer](https://github.com/blader/humanizer)（原始專案）
- [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop)（參考）
- [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh)（原始翻譯版）
