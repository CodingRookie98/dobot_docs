# DobotLink API 文档（中文版本）

本目录包含从 `DobotLinkHelp.CHM` 转换而来的中文版本 DobotLink API 文档。

## 文档统计

- **总文件数**：778 个 Markdown 文件（含本 README）
- **API 文档数**：777 个
- **索引文件**：[index.md](./index.md) - 按字母顺序列出所有 API 文档

## 目录结构

```
./
├── index.md               完整文档索引
├── 1 前言/                 前言/开发协议说明
├── 2 DobotLink API/       DobotLink 核心 API
├── 3 Magician API/        Magician 相关 API
├── 4 MagicianLite API/    MagicianLite 相关 API
├── 5 MagicBox API/        MagicBox 相关 API
├── 6 M1 API/              M1 机器人相关 API
├── 7 CR API/              CR 控制器相关 API
├── 8 MagicianPro API/     MagicianPro 相关 API
├── 9 MagicianGO API/      MagicianGO 相关 API
├── 10 DebuggerLite API/   调试器相关 API
├── 11 Download API/       下载与固件升级相关 API
└── 13 错误码/              错误码说明
```

## 文件分类说明

| 分类 | 说明 |
|------|------|
| [`index.md`](./index.md) | 完整文档索引，按字母顺序排列所有文档链接 |
| [`1 前言/`](./1%20前言) | 协议说明与开发前言说明 |
| [`2 DobotLink API/`](./2%20DobotLink%20API), [`10 DebuggerLite API/`](./10%20DebuggerLite%20API), [`11 Download API/`](./11%20Download%20API), [`13 错误码/`](./13%20错误码) | 核心功能、调试工具、下载以及错误码通用模块 |
| [`3 Magician API/`](./3%20Magician%20API) 至 [`9 MagicianGO API/`](./9%20MagicianGO%20API) | 按机械臂或机器人硬件型号分类的专用 API 文档 |

## 转换说明

本文档由原始 CHM 帮助文件转换而来：

- **来源**：`DobotLinkHelp.CHM`
- **转换工具**：`extract_chmLib` + `pandoc`
- **编码处理**：GBK → UTF-8 转换，确保中文正确显示
- **整理时间**：2026-04-16（于 2026-05-26 完成全面复核与死链修复）

## 验证状态

✅ 所有 777 个 API 文档转换完成
✅ 中文编码正确，可正常阅读
✅ 索引完整，包含所有文档链接
✅ 目录结构与英文版本完全一致
✅ 已删除无内容占位页面

---

## 📝 修复与更新日志

### 2026-05-26
- **补齐缺失 API 文档**：补齐了原本缺失的 `SetTraceLoop`（设置巡线循环使能）接口说明文档：[SetTraceLoop](./9%20MagicianGO%20API/9.4%20%E5%BA%95%E7%9B%98%E6%8E%A7%E5%88%B6(control)/SetTraceLoop.md)，并在 [index.md](./index.md) 中配置了对应的字母索引链接。
