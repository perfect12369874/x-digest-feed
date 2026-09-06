# X 情报 Feed

每天写入 `data/latest.json` 并 push 到 GitHub Pages。

字段：date, updated_at, related[], hot[]。
每条：author, text（中文主文）, text_zh, text_en（原文）, why, heat, url, media[]。
页面优先展示中文，附原文。
