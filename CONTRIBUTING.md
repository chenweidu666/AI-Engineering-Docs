# 参与与编辑说明

- **站内可见内容**：由根目录 **`_sidebar.md`** 定义，对应 `docs/` 下七章主线（`01_基础层` … `07_项目总结`）。说明见 [docs/README.md](./docs/README.md)。
- **上游镜像（CineMaker / OpenClaw）**：`python3 scripts/fetch_github_docs.py` 默认写入 **`../归档/from_3_技术文档/projects/`**。Docsify 正文入口在 **`docs/07_项目总结/7.1_CineMaker/`** 与 **`docs/07_项目总结/7.2_OpenClaw-Deployment-Issues/`**；上游更新后请将脚本产出与上述目录对齐（复制或沿用你本地的同步流程），侧栏见根目录 **`_sidebar.md`**。
- **已迁出归档**：旧版 `01_模型训练与微调`、`02_模型部署与推理`、`03_RAG检索增强生成`、`04_Agent智能体开发`、`05_AI编译器与底层优化`、`06_工程化与服务部署` 及上述 `projects` 镜像，见 **`../归档/from_3_技术文档/`**。
- **Docsify 首页**：`index.html` 中 `homepage: docs/README.md`；全文搜索使用 `paths: "auto"`，覆盖当前 `docs/` 内 Markdown。
