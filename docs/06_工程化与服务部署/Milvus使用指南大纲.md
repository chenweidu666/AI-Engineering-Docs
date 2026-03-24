# Milvus 向量数据库使用指南

> 对应简历：RAG & 向量检索 · Milvus · 太初（2024-2025）

## 目录

1. 向量数据库的作用（语义检索 vs 关键词检索）
2. Milvus核心概念
   - Collection / Field / Index / Metric Type
   - 索引类型：IVF_FLAT / HNSW / IVF_SQ8
3. 安装部署（Docker单机）
4. Python SDK实战
   - 连接、创建集合、插入向量、构建索引、查询
5. 在RAG中的完整链路
6. 性能调优与索引选型
7. 与Chroma/Faiss对比
