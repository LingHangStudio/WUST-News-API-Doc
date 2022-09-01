# 新闻列表

获取初始新闻列表，或更新新闻列表。本接口适用于学校、教务、团委板块。

## 路径

```
/post/news-list
```

## 请求

```json
{
	"part": 1,
	"sub": 1,
	"num": 20,
	"page": 0
}
```

- `part`：所属的大类，学校、教务、学院、团委，编号从 1 开始
- `sub`：大类中的小类，编号从 1 开始
- `num`：每页的新闻条数
- `page`：分页号，从 0 开始

## 响应

```json
{
	"part": 1,
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

- `part` , `sub` , `num` , `page` 为请求的数据
- `databaseUpdateTime`：最后一次爬虫开始运行的时间戳
- `newsList`：新闻列表，新闻对象的列表
- `id`：新闻的唯一标识符
- `title`：新闻的标题字符串
- `date`：新闻的日期
- `picList`：新闻中包含的图片列表，每项为图片的 URL 字符串

## 编号

### 大类编号

| 编号 | 名称 | 拼音 |
| --- | --- | --- |
| 1 | 学院 | xueyuan |
| 2 | 教务 | jiaowu |
| 4 | 团委 | tuanwei |

### 小类编号

#### 学院 (1)

| 编号 | 名称 | 拼音 |
| --- | --- | --- |
| 1 | 要闻 | yaowen |
| 2 | 媒体 | meiti |
| 3 | 学术 | xueshu |
| 4 | 综合 | zonghe |
| 5 | 院系 | yuanxi |

### 教务 (2)

| 编号 | 名称 | 拼音 |
| --- | --- | --- |
| 1 | 通知公告 | tongzhigonggao |
| 2 | 教学动态 | jiaoxuedongtai |

### 团委 (4)

| 编号 | 名称 | 拼音 |
| --- | --- | --- |
| 1 | 团情 | tuanqing |
| 2 | 基层信息 | jicengxinxi |
| 3 | 文件资料 | wenjianziliao |
| 4 | 学生活动 | xueshenghuodong |
| 5 | 热点聚焦 | redianjujiao |
| 6 | 他山之石 | tashanzhishi |
