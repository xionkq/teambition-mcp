# teambition-mcp

仿照官方实例写的，用于学习目的

## 如何使用

1. 登录 teambition，在你的组织中新建一个应用
2. 给予应用读取任务权限
3. 获取应用 id、应用密码、操作者 id、组织 id
4. 将本仓库 build/index.js 文件下载到本地
5. 在 cursor mcp.json 中输入添加如下配置
```json
{
  "mcpServers": {
    "teambition-mcp": {
      "command": "node",
      "args": [
        "\\path\\to\\the\\local\\index.js",
        "应用 id",
        "应用密码",
        "操作者 id",
        "组织 id"
      ]
    }
  }
}
```
6. 在 cursor setting 中启用 teambition-mcp
