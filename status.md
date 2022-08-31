# 服务状态

报告当前服务状态，通过 GET 方法请求。

## 路径

```
/status
```

## 响应

```json
{
	"status": "running"
}
```

- `status`：当前服务状态，`'running'` 表示正在运行，`'maintaining'` 表示正在维护。
