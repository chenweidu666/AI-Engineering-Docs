# 参与与编辑说明

- **站内可见内容**：由根目录 **`_sidebar.md`** 定义，对应 `docs/` 下七章主线（`01_基础层` … `07_项目总结`）。说明见 [docs/README.md](./docs/README.md)。
- **上游镜像（CineMaker / OpenClaw）**：同步脚本写入 **`1_陈纬简历/归档/from_3_技术文档/projects/`**，不再放在 `docs/projects/`。源仓库修改后执行 `python3 scripts/fetch_github_docs.py`；若需把这些文档重新挂进 Docsify，请自行在 `_sidebar.md` 增加链接或迁回 `docs/`。
- **已迁出归档**：旧版 `01_模型训练与微调`、`02_模型部署与推理`、`03_RAG检索增强生成`、`04_Agent智能体开发`、`05_AI编译器与底层优化`、`06_工程化与服务部署` 及上述 `projects` 镜像，见 **`../归档/from_3_技术文档/`**。
- **Docsify 首页**：`index.html` 中 `homepage: docs/README.md`；全文搜索使用 `paths: "auto"`，覆盖当前 `docs/` 内 Markdown。
