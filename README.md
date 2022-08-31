# 武科大助手新闻资讯 API 文档

本文档为武科大助手新闻资讯 API 文档

## 新闻标识符

每条新闻在数据库中有唯一的 `id` ，根据 `id` 来标识不同的新闻。不论数据库怎样更新，`id` 值不再改变。

## 接口命名规范

### 接口类型

GET 接口挂载于

```
http://example.com/get/
```

POST 接口挂载于

```
http://example.com/post/
```

服务状态接口

```
http://example.com/status
```

### 接口命名

用短线法命名，例如：

```
http://example.com/get/read-count
http://example.com/post/news-list
```

### 响应字段命名

用小驼峰法命名，例如：

```json
{
	"id": "7001",
	"title": "我校获第十届全国大学生机械创新设计大赛一等奖",
	"readCounter": 100,
	"likeCounter": 25
}
```
