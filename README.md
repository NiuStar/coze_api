# coze_api
接口：```https://cozeapi.ai00.xyz/coze_api/send```

参数：
```json
{
	"bot_id": "7319498133556428806",
	"local_message_id": "R55a6JfSBafgckKRzQS0Z",
	"content_type": "text",
	"query": "你好",
	"extra": {},
	"scene": 2,
	"bot_version": "1708583912973",
	"stream": true,
	"chat_history": []
}
```
header中添加auth头，及coze的sessionId
例如：
<img width="982" alt="image" src="https://github.com/NiuStar/coze_api/assets/16755722/d767bd7e-c4f9-404c-a207-3caf69e80c1e">


内测阶段，auth头请发送申请至yjkj02@gmail.com。
目前不知道coze的请求上限，小范围试用，请见谅

说明文档
```
id为uuid，随意生成就可以
sessionId第一次会话不需要传，会返回回来一个，类似于chatgpt的conversationId，是拿来做会话隔离用的
sender是非必传字段，是为了人性化的回复，比如说你的sender是张三，ai就知道会话的人叫做张三，所以这个如果是做微信或者tg等聊天机器人的时候
会有用
```
