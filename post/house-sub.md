# 学院板块列表

考虑到各个学院新闻网站分类不一样，故设置该接口用于查询学院有哪些板块及编号

## 路径

```
/post/house-sub
```

## 请求

```json
{
	"house": 1
}
```

- `house`：学院编号

## 响应

```json
{
	"house": 1,
	"subList": [
		{
			"sub": 1,
			"name": "公告"
		},
		{
			"sub": 2,
			"name": "新闻"
		}
	]
}
```

- `house`：学院编号
- `subList`：学院的板块列表，每项为板块对象
- `sub`：板块的编号数字
- `name`：板块的名称字符串

## 学院编号

| 编号 | 学院 | 拼音 |
| --- | --- | --- |
| 1 | 材料与冶金学院 | cailiaoyuyejinxueyuan |
| 2 | 城市建设学院 | chengshijianshexueyuan |
| 3 | 恒大管理学院 | hengdaguanlixueyuan |
| 4 | 国际学院 | guojixueyuan |
| 5 | 化学与化工学院 | huaxueyuhuagongxueyuan |
| 6 | 机械自动化学院 | jixiezidonghuaxueyuan |
| 7 | 计算机科学与技术学院 | jisuanjikexueyujishuxueyuan |
| 8 | 理学院 | lixueyuan |
| 9 | 马克思主义学院（临床学院忽略） | makesizhuyixueyuan |
| 10 | 汽车与交通工程学院 | qicheyujiaotonggongchengxueyuan |
| 11 | 生命科学与健康学院 | shengmingkexueyujiankangxueyuan |
| 12 | 体育学院 | tiyuxueyuan |
| 13 | 外国语学院 | waiguoyuxueyuan |
| 14 | 文法与经济学院 | wenfayujingjixueyuan |
| 15 | 信息科学与工程学院 | xinxikexueyugongchengxueyuan |
| 16 | 医学院（公共卫生学院忽略） | yixueyuan |
| 17 | 艺术与设计学院 | yishuyushejixueyuan |
| 18 | 资源与环境工程学院 | ziyuanyuhuanjinggongchengxueyuan |
