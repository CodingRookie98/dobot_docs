# DobotLink API 文档

本目录包含 DobotLink API 文档的不同语言版本，以及相关文档。

## 目录结构

```
./
├── DobotLinkHelp/                  中文版本 API 文档（从 DobotLinkHelp.CHM 转换整理）
├── DobotLinkHelp_EN/               英文版本 API 文档（从 DobotLinkHelp_EN.CHM 转换整理）
├── Dobot_edu_api.md                DobotEDU Python SDK 接口文档
└── Dobot_TCP_IP二次开发接口文档...  Dobot TCP/IP 协议二次开发接口官方文档（Markdown版本）
```

## 版本说明

### DobotLink API

- **DobotLinkHelp/**：完整整理的中文版本 API 文档，所有目录已按 `章节序号+章节名` 重命名，所有文件已清理冗余模板标记，`index.md` 包含完整索引
- **DobotLinkHelp_EN/**：完整整理的英文版本 API 文档，结构与中文版本完全一致，所有中文目录名称已修正为正确中文
- 进入对应目录后查看 `index.md` 获取完整文档索引

### 额外文档

- **Dobot_edu_api.md**：DobotEDU Python SDK 接口文档
- **Dobot_TCP_IP二次开发接口文档V4.6.0_2024.12.26_cn.md**：Dobot TCP/IP 协议二次开发接口官方文档（已转换为 Markdown）

## 处理说明

两个 CHM 文档都经过以下完整流程处理：
1. 解压 CHM → HTML → 转换为 Markdown
2. 递归重命名所有目录至 `章节序号+章节名称` 格式，层级关系保持一致
3. 所有零散文件整理到对应子章节目录
4. 清理所有 EasyCHM 模板容器标记、导航链接、水印、冗余CSS样式
5. 标准化文档格式，提取标题并设置对应层级
6. 生成/更新 `index.md` 并修复所有链接
7. 所有修改已提交 Git 保留完整历史
