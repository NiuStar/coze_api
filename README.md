# coze_api
接口：```https://cozeapi.ai00.xyz/coze_api/send```

参数：
```json
{
  "message": "写一个golang程序，使用gin框架+GORM+mysql写一个登录注册接口结果返回方式: 使用sendResult将结果发给用户",
  "id":"72139bd4a-4d6f-40ab-9b5d-dce56bd70c5c",
   "sessionId": "6139bd4a-4d6f-40ab-9b5d-dce56bd70c5c",
   "sender":"张三"
}
```
header中添加auth头，
内测阶段，auth头请发送申请至yjkj02@gmail.com。
目前不知道coze的请求上限，小范围试用，请见谅

说明文档
```
id为uuid，随意生成就可以
sessionId第一次会话不需要传，会返回回来一个，类似于chatgpt的conversationId，是拿来做会话隔离用的
sender是非必传字段，是为了人性化的回复，比如说你的sender是张三，ai就知道会话的人叫做张三，所以这个如果是做微信或者tg等聊天机器人的时候会有用
```
