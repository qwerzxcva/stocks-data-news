# stocks-data-news (财经新闻档案)

## 用途
7×24 财经新闻抓取 + 按日归档 + 已读 ID 去重。用于复盘和消息面分析。

## 数据来源
新浪 7×24 `app.cj.sina.com.cn/api/news/pc`

## 目录结构
```
news/
  YYYY-MM-DD.md        每日新闻 (7x24 格式, 带时间戳和分类标签)
  .seen_ids.txt        已读新闻 ID 列表 (去重用)
```

## 采集
运行: `python3 ~/workspace/stocks-tools/tools/news_collect.py` (需要传入仓库 root 参数)
或直接跑 `bash ~/workspace/stocks-tools/tools/news_loop.sh` 做周期性抓取。
