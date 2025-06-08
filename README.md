# GitHub Action 测试项目

这个项目用于测试 GitHub Actions 的功能，特别是实现了一个简单的通知功能。

## 功能说明

当代码推送到主分支时，会自动触发 GitHub Action，向指定的 ntfy 服务器发送通知消息。

## 配置要求

在 GitHub 仓库的 Secrets 中需要配置以下参数：

- `NTFY_SERVER`: ntfy 服务器地址
- `NTFY_PORT`: ntfy 服务器端口
- `NTFY_TOPIC`: 通知主题
- `NTFY_TOKEN`: 验证令牌

## 使用方法

1. 确保已在 GitHub 仓库中配置了所需的 Secrets
2. 将代码推送到主分支
3. GitHub Action 将自动触发并发送通知

## 注意事项

- 请确保 ntfy 服务器配置正确且可访问
- 验证令牌需要具有发送消息的权限 