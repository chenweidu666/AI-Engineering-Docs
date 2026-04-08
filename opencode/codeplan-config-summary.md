# OpenCode + Claude CodePlan 配置总结

## 配置信息

### API 信息
- **API 密钥**: `sk-sp-4a72cbac7f5d407eb9e0041e234fb563`
- **Anthropic 兼容接口**: `https://coding.dashscope.aliyuncs.com/apps/anthropic`
- **OpenAI 兼容接口**: `https://coding.dashscope.aliyuncs.com/v1`
- **模型**: `qwen3.5-plus`

## 1. OpenCode 配置

### 配置文件
文件路径: `~/.config/opencode/opencode.json`

```json
{
  "$schema": "https://opencode.ai/config.json",
  "provider": {
    "anthropic": {
      "options": {
        "apiKey": "sk-sp-4a72cbac7f5d407eb9e0041e234fb563",
        "baseURL": "https://coding.dashscope.aliyuncs.com/apps/anthropic"
      }
    }
  },
  "model": "anthropic/claude-sonnet-4-5"
}
```

### 环境变量
添加到 `~/.zshrc` 或 `~/.bashrc`:

```bash
# OpenCode / Claude CodePlan Configuration
export CLAUDE_API_KEY=sk-sp-4a72cbac7f5d407eb9e0041e234fb563
export CLAUDE_BASE_URL=https://coding.dashscope.aliyuncs.com/apps/anthropic
export CLAUDE_MODEL=qwen3.5-plus
export ANTHROPIC_API_KEY=sk-sp-4a72cbac7f5d407eb9e0041e234fb563
export ANTHROPIC_BASE_URL=https://coding.dashscope.aliyuncs.com/apps/anthropic
```

## 2. Claude CLI 配置

如果使用 Claude CLI，可以设置环境变量:

```bash
export ANTHROPIC_API_KEY=sk-sp-4a72cbac7f5d407eb9e0041e234fb563
export ANTHROPIC_BASE_URL=https://coding.dashscope.aliyuncs.com/apps/anthropic
```

## 3. 测试连接

### 使用 curl 测试
```bash
curl -s "https://coding.dashscope.aliyuncs.com/apps/anthropic/v1/messages" \
  -H "Content-Type: application/json" \
  -H "x-api-key: sk-sp-4a72cbac7f5d407eb9e0041e234fb563" \
  -H "anthropic-version: 2023-06-01" \
  -d '{
    "model": "qwen3.5-plus",
    "max_tokens": 1024,
    "messages": [
      {"role": "user", "content": "你好"}
    ]
  }'
```

### 使用 OpenCode 测试
```bash
opencode run "你好"
```

## 4. 注意事项

### ⚠️ 已知限制
1. **OpenCode 模型选择**: OpenCode 的 `anthropic` 提供商只支持官方 Claude 模型列表，不支持自定义的 `qwen3.5-plus` 模型标识
2. **替代方案**: 可以通过 API 直接调用，或使用其他支持自定义 Anthropic 端点的客户端

### ✅ 测试成功的连接方式
- **curl 直接调用**: ✅ 成功
- **API 响应**: 正常返回中文回复
- **模型**: `qwen3.5-plus` 可用

## 5. 相关资源

- [阿里云 CodePlan 文档](https://help.aliyun.com/zh/model-studio/coding-plan-faq)
- [Anthropic API 文档](https://docs.anthropic.com/)
- [OpenCode 文档](https://opencode.ai/docs)

## 6. 配置日期

- **配置日期**: 2026-04-08
- **测试状态**: API 连接成功 ✅
