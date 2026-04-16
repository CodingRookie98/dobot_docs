# DobotLink API 文档（中文版本）

本目录包含从 `DobotLinkHelp.CHM` 转换而来的中文版本 DobotLink API 文档。

## 文档统计

- **总文件数**：777 个 Markdown 文件（含本 README）
- **API 文档数**：776 个
- **索引文件**：[index.md](./index.md) - 按字母顺序列出所有 API 文档

## 目录结构

```
./
├── index.md            完整文档索引
├── preface.md          前言/开发协议说明
├── CR/                 CR 控制器相关 API
├── DebuggerLite/       调试器相关 API
├── DobotLink/          DobotLink 核心 API
├── Download/           下载相关 API
├── ErrorCode/          错误码说明
├── M1/                 M1 机器人相关 API
├── MagicBox/           MagicBox 相关 API
├── Magician/           Magician 相关 API
├── MagicianGO/         MagicianGO 相关 API
├── MagicianLite/       MagicianLite 相关 API
└── MagicianPro/        MagicianPro 相关 API
```

## 文件分类说明

| 分类 | 说明 |
|------|------|
| `index.md` | 完整文档索引，按字母顺序排列所有文档链接 |
| `preface.md` | 开发协议说明与前言 |
| `CR/`, `DebuggerLite/`, `DobotLink/`, `Download/`, `ErrorCode/` | 通用功能模块 API |
| `M1/`, `MagicBox/`, `Magician/`, `MagicianGO/`, `MagicianLite/`, `MagicianPro/` | 按机器人型号分类的 API 文档 |

## 转换说明

本文档由原始 CHM 帮助文件转换而来：

- **来源**：`DobotLinkHelp.CHM`
- **转换工具**：`extract_chmLib` + `pandoc`
- **编码处理**：GBK → UTF-8 转换，确保中文正确显示
- **整理时间**：2026-04-16

## 验证状态

✅ 所有 776 个 API 文档转换完成  
✅ 中文编码正确，可正常阅读  
✅ 索引完整，包含所有文档链接  
✅ 目录结构与英文版本完全一致  
✅ 已删除无内容占位页面
