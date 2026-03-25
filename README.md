# AI-Engineering-Docs · CW Tech Docs

AI 工程技术文档站，按大模型完整技术栈组织，共八章（第七、八章为项目长篇文档子站）。

[![GitHub Pages](https://img.shields.io/badge/在线阅读-GitHub%20Pages-0366d6?logo=github)](https://chenweidu666.github.io/AI-Engineering-Docs/)
[![Resume](https://img.shields.io/badge/简历-Resume--Site-2563EB?logo=github)](https://chenweidu666.github.io/Resume-Site/)

## 在线阅读

**👉 https://chenweidu666.github.io/AI-Engineering-Docs/**

## 文档结构

| 章节 | 内容 |
|------|------|
| 一、基础层 | 1.1–1.4：动机与缩放 / Transformer / 主流选型 / 趋势与参考 |
| 二、训练与微调 | 数据处理与预训练 / SFT / LoRA / RLHF / 分布式训练 |
| 三、部署与推理 | KV Cache 与推理加速 / vLLM / INT 量化 |
| 四、RAG 与知识库 | 4.1：RAG、Milvus 与 LangChain（单篇） |
| 五、Agent 开发 | 工作流 / MCP / Dify / AppAgent（OpenClaw 见第七、八章） |
| 六、工程化 | FastAPI / Docker 容器化 |
| 七、项目总结 | CineMaker 手册 · OpenClaw 部署实录（[`docs/07_项目总结/`](docs/07_项目总结/README.md)） |
| **八、OpenClaw 实战系列** 🆕 | Dashboard 部署 / 双龙虾架构 / Git 同步 / MCP 集成 / BTC 量化策略（[`docs/08_OpenClaw 实战/`](docs/08_OpenClaw 实战/)） |

## 仓库结构

```
├── docs/
│   ├── README.md                 # 站点首页
│   ├── 01_基础层/
│   ├── 02_训练与微调/
│   ├── 03_部署与推理/
│   ├── 04_RAG 与知识库/
│   ├── 05_Agent 开发/
│   ├── 06_工程化/
│   ├── 07_项目总结/              # CineMaker / OpenClaw 镜像文档（见 README）
│   └── 08_OpenClaw 实战/         # OpenClaw 实战系列（8 篇）
├── index.html                    # Docsify 配置
├── _sidebar.md                   # 侧边栏导航
└── README.md                     # 本文件
```

## 新增内容

### 🦞 OpenClaw 实战系列（第八章）

2026-03-25 新增 8 篇实战文档：

1. Dashboard 部署与移动端优化
2. 双龙虾架构设计与实现
3. Git 记忆同步机制详解
4. OpenClaw 本地部署指南
5. Gate 交易所 MCP 集成
6. BTC 量化交易策略实录
7. OpenClaw 技能开发指南
8. 常见问题与故障排查

**总计约 62,500 字**，涵盖 OpenClaw 从部署到实战的完整流程。

## 联系

- 📧 [514351508@qq.com](mailto:514351508@qq.com)
- 💼 [简历](https://chenweidu666.github.io/Resume-Site/)
- 🐙 [github.com/chenweidu666](https://github.com/chenweidu666)
