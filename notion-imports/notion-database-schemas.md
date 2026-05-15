# Notion Database Schemas｜星座星盤資料庫欄位結構

此檔案整理自 Notion「星座星盤」主頁下的資料庫結構。

## 星體資料庫

Notion 資料庫名稱：星體

資料庫用途：整理星體名稱、類別、驅動力與詳細說明。

| 欄位 | 類型 | 說明 |
|---|---|---|
| 名稱 | title | 星體名稱 |
| 類別 | text | 星體分類，例如個人星、社會星、世代星等 |
| 驅動力 | text | 該星體代表的核心驅動力 |
| 驅動力詳解 | text | 對驅動力的補充說明 |

建議 GitHub 對應位置：

```text
planets/
keywords/planet-keywords-table.md
```

## 宮位資料庫

Notion 資料庫名稱：宮位

資料庫用途：整理十二宮位與生活場景。

| 欄位 | 類型 | 說明 |
|---|---|---|
| 名稱 | title | 宮位名稱 |
| 宮位 | text | 宮位編號或名稱 |
| 星體能量發生在哪個生活場景 | text | 該宮位代表的生活領域 |

建議 GitHub 對應位置：

```text
houses/
keywords/house-keywords-table.md
```

## 相位資料庫

Notion 資料庫名稱：相位

資料庫用途：整理相位名稱、角度與能量互動方式。

| 欄位 | 類型 | 說明 |
|---|---|---|
| 名稱 | title | 相位名稱 |
| 度數 | text | 相位角度，例如 0°、60°、90°、120°、180° |
| 星體能量發生在哪個生活場景 | text | 原資料庫欄位名如此，實際上可理解為相位能量互動說明 |

建議 GitHub 對應位置：

```text
aspects/
keywords/aspect-keywords-table.md
```

## 後續整理建議

若要讓 GitHub 知識庫更完整，建議接著新增：

```text
houses/
├── 00-overview.md
├── house-01.md
├── house-02.md
├── house-03.md
├── house-04.md
├── house-05.md
├── house-06.md
├── house-07.md
├── house-08.md
├── house-09.md
├── house-10.md
├── house-11.md
└── house-12.md

aspects/
├── 00-overview.md
├── conjunction.md
├── sextile.md
├── square.md
├── trine.md
├── opposition.md
├── sesquiquadrate.md
└── quincunx.md
```

## 搬移狀態

目前已搬移：

- 星體資料庫 schema
- 宮位資料庫 schema
- 相位資料庫 schema

目前尚未完整搬移：

- 星體資料庫所有資料列
- 宮位資料庫所有資料列
- 相位資料庫所有資料列

原因：目前 Notion 連接器可讀取資料庫 schema，但資料庫 row 查詢工具在本次操作中無法正常使用。若之後可匯出 Markdown/CSV，或資料庫 row 可被完整 fetch，便可補齊。
