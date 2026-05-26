# DobotLink API Documentation (English Version)

This directory contains the English version of the DobotLink API documentation, converted and perfected from the original `DobotLinkHelp_EN.CHM` compiled help file.

## Documentation Statistics

- **Total Files**: 778 Markdown files (including this README)
- **API Pages**: 777 documents
- **Main Index**: [`index.md`](./index.md) - Alphabetical list of all available API pages

## Directory Structure

```
./
├── index.md               Complete document index
├── 1 前言/                 Preface / Development protocol description
├── 2 DobotLink API/       DobotLink core APIs
├── 3 Magician API/        Magician APIs
├── 4 MagicianLite API/    MagicianLite APIs
├── 5 MagicBox API/        MagicBox APIs
├── 6 M1 API/              M1 Robot APIs
├── 7 CR API/              CR Controller APIs
├── 8 MagicianPro API/     MagicianPro APIs
├── 9 MagicianGO API/      MagicianGO APIs
├── 10 DebuggerLite API/   DebuggerLite APIs
├── 11 Download API/       Firmware download & upgrade APIs
└── 13 Error Code/         Error code specifications
```

## File Classifications

| Category | Description |
|------|------|
| [`index.md`](./index.md) | The complete alphabetical index of all API links. |
| [`1 前言/`](./1%20前言) | Protocol explanations and introduction. |
| [`2 DobotLink API/`](./2%20DobotLink%20API), [`10 DebuggerLite API/`](./10%20DebuggerLite%20API), [`11 Download API/`](./11%20Download%20API), [`13 Error Code/`](./13%20Error%20Code) | General helper modules including core APIs, debugging tools, download services, and error codes. |
| [`3 Magician API/`](./3%20Magician%20API) to [`9 MagicianGO API/`](./9%20MagicianGO%20API) | Specific robot model API suites (arranged by hardware type). |

## Conversion Details

This documentation subset has been converted and audited from:

- **Source File**: `DobotLinkHelp_EN.CHM`
- **Tooling**: `extract_chmLib` + `pandoc`
- **Encoding**: GBK / CP936 to UTF-8 conversion, ensuring code snippets and comments display correctly.
- **Audit Date**: 2026-05-26 (Checked and fixed 269 empty Markdown pages).

## Verification Status

✅ All 777 API documents fully converted
✅ Character encoding corrected, 100% readable
✅ Index fully configured with portable links
✅ Empty and corrupted pages completely resolved
✅ Zero dead links / absolute path issues

---

## 📝 Update & Bugfix Log

### 2026-05-26
- **Completed Missing API Documentation**:
  - Added documentation for `dobotlink.MagicianGO.SetTraceLoop` (which was missing from the official CHM release): [SetTraceLoop](./9%20MagicianGO%20API/9.4%20%E5%BA%95%E7%9B%98%E6%8E%A7%E5%88%B6(control)/SetTraceLoop.md).
  - Added the alphabetical index link in [index.md](./index.md).
- **Corrected Typographic Errors in English API Documents**:
  - **`ConnectDobot`**: Fixed the incorrect JSON-RPC method name `dobotlink.MagicianPro.ConnectDobot` -> `dobotlink.MagicianGO.ConnectDobot` in [ConnectDobot](./9%20MagicianGO%20API/9.1%20%E8%AE%BE%E5%A4%87%E8%BF%9E%E6%8E%A5(connect)/ConnectDobot.md).
  - **`SetRunningMode`**: Fixed the incorrect parameter name `runningState` -> `runningMode` in [SetRunningMode](./9%20MagicianGO%20API/9.4%20%E5%BA%95%E7%9B%98%E6%8E%A7%E5%88%B6(control)/SetRunningMode.md).
