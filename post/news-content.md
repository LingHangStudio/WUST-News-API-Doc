# 新闻正文

获取新闻正文，以及新闻的其他信息。

## 路径

```
/post/news-content
```

## 请求

```json
{
	"id": "7001"
}
```

- `id`：文章的唯一标识符

## 响应

```json
{
	"id": "7001",
	"title": "我校获第十届全国大学生机械创新设计大赛一等奖",
	"date": {
		"year": 2022,
		"month": 8,
		"day": 25
	},
	"readCounter": 100,
	"likeCounter": 50,
	"commentCounter": 3,
	"content": "<div> ... </div>",
	"picList": [
		"https://wust.edu.cn/pic1.jpg",
		"https://wust.edu.cn/pic2.jpg",
		"https://wust.edu.cn/pic3.jpg"
	],
	"fileList": [
		"https://wust.edu.cn/doc1.docx"
	]
}
```

- `id`：文章的唯一标识符
- `title`：新闻的标题字符串
- `date`：新闻的日期
- `readCounter`：阅读次数，为官网阅读次数与助手阅读次数之和（暂不实现）
- `likeCounter`：点赞次数（暂不实现）
- `commentCounter`：评论条数（暂不实现）
- `content`：新闻的 HTML 正文部分
- `picList`：新闻所含的图片列表，每项为图片 URL 字符串。若无图片，则返回空列表
- `fileList`：新闻所含的附件列表，每项为附件的 URL 字符串。若无附件，则返回空列表
