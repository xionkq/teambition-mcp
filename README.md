# teambition-mcp

A project created for learning purposes by imitating official examples

## How to Use

1. Log in to Teambition and create a new app in your organization
2. Grant the app Read task permissions
3. Obtain the App ID, App Secret, Operator ID, and Organization ID
4. Download the build/index.js file from this repository to your local machine
5. Add the following configuration in cursor mcp.json:
```json
{
  "mcpServers": {
    "teambition-mcp": {
      "command": "node",
      "args": [
        "/path/to/the/local/index.js",
        "App ID",
        "App Secret",
        "Operator ID",
        "Organization ID"
      ]
    }
  }
}
```
6. Enable teambition-mcp in cursor settings
