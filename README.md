# Kotlin 协程深度指南

面向 Android 开发者的 Kotlin 协程学习站点，覆盖 `suspend` 状态机、结构化并发、异常处理、Flow、Android 架构落地、测试、性能反模式和大厂面试题。

## 本地运行

```bash
npm install
npm start
```

默认访问：

```text
http://localhost:3000
```

如需指定端口：

```bash
PORT=3002 npm start
```

Windows PowerShell 如果阻止 `npm.ps1`，使用：

```powershell
npm.cmd start
```

## Railway 部署

项目已包含 Railway 所需配置：

- `server.js`：读取 Railway 注入的 `PORT` 并提供静态页面
- `package.json`：`npm start` 启动命令
- `railway.json`：Nixpacks 构建和启动配置

部署方式：

```bash
npm i -g @railway/cli
railway login
railway init
railway up
```

在非交互终端中，Railway CLI 需要 token：

```powershell
$env:RAILWAY_TOKEN="your-token"
railway.cmd init
railway.cmd up
```

也可以使用 `RAILWAY_API_TOKEN`。
