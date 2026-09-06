# X 情报 Feed（含往期归档）

- 最新：`data/latest.json`
- 索引：`data/index.json`（daily / weekly / monthly 列表）
- 归档：`data/daily/YYYY-MM-DD.json`、`data/weekly/YYYY-Www.json`、`data/monthly/YYYY-MM.json`

每期字段含 kind/period/label，条目含中文 text/text_zh、原文 text_en、media。
每次推送后更新对应归档文件、index.json，并同步 latest.json（每日默认）。
