# X 情报 Feed

X 情报每天写入 `data/latest.json`（并 push 到 GitHub Pages 仓库）。

## latest.json 格式

```json
{
  "date": "2026-09-06",
  "updated_at": "2026-09-06T10:00:00+08:00",
  "related": [
    {
      "author": "@handle · Name",
      "text": "足够原文，用户不用点出去也能读懂",
      "why": "为何相关（一句）",
      "heat": "热度线索",
      "url": "https://x.com/...",
      "media": [
        {
          "type": "photo",
          "url": "https://pbs.twimg.com/media/....jpg",
          "preview_url": ""
        },
        {
          "type": "video",
          "url": "https://video.twimg.com/...mp4",
          "preview_url": "https://pbs.twimg.com/...."
        }
      ]
    }
  ],
  "hot": []
}
```

`related` ≈ A 相关 20；`hot` ≈ B 全站最热 20。
`media` 可选：有图/视频时从 X API `attachments.media_keys` + `media.fields` 写入直链；页面直接展示。
