# DeployPlatform
***
## 效果
- 前端输入集群名、集群的角色、地址、apinfo进行集群部署
- 开始部署后可以通过前端看到实时的日志响应
## 技术特点
- django 2.1.11
- celery进行异步处理
- redis缓存前端的部署信息
- paramiko进行文件的传输和命令的执行
- channels进行websocket连接
- rabbitmq缓存执行命令后的日志信息
- 部署：nginx（http）+daphne（websocket）
