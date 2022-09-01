# 搜索新闻

## 路径

```
/post/search-news
```

## 请求

```json
{
	"keyword": "运动会"
}
```

- `keyword`：搜索关键字

## 响应

```json
{
	"keyword": "运动会",
	"newsList": [
		{
			"id": 7001,
			"title": "我校获第十届全国大学生机械创新设计大赛一等奖",
			"date": {
				"year": 2022,
				"month": 8,
				"day": 25
			},
			"picList": [
				"https://wust.edu.cn/pic1.jpg",
				"https://wust.edu.cn/pic2.jpg",
				"https://wust.edu.cn/pic3.jpg"
			]
		}
	]
}
```

- `keyword`：搜索关键字
- `newsList`：新闻列表，新闻对象的列表，最多 20 个，若无匹配则返回空列表
- `id`：新闻的唯一标识符
- `title`：新闻的标题字符串
- `date`：新闻的日期
- `picList`：新闻中包含的图片列表，每项为图片的 URL 字符串
