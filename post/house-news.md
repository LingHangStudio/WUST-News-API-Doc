# 学院新闻列表

获取初始新闻列表，或更新新闻列表。本接口适用于学院板块。

## 路径

```
/post/house-news
```

## 请求

```json
{
	"house": 1,
	"sub": 1,
	"num": 20,
	"page": 0
}
```

- `house`：学院编号
- `sub`：大类中的小类，编号从 1 开始
- `num`：每页的新闻条数
- `page`：分页号，从 0 开始

## 响应

```json
{
	"house": 1,
	"sub": 1,
	"num": 20,
	"page": 0,
	"databaseUpdateTime": 10000001,
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

- `house` , `sub` , `num` , `page` 为请求的数据
- `databaseUpdateTime`：最后一次爬虫开始运行的时间戳
- `newsList`：新闻列表，新闻对象的列表
- `id`：新闻的唯一标识符
- `title`：新闻的标题字符串
- `date`：新闻的日期
- `picList`：新闻中包含的图片列表，每项为图片的 URL 字符串
