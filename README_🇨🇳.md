# OWASP WSTG 评估工具与检查清单编辑器

![OWASP WSTG Assessment](https://img.shields.io/badge/OWASP-WSTG%20Assessment-blue.svg)
![Version](https://img.shields.io/badge/version-3.0-green.svg)
![License](https://img.shields.io/badge/license-MIT-orange.svg)
![RTL Support](https://img.shields.io/badge/RTL-Supported-success.svg)

这是一个基于网页、完全在客户端运行且支持离线的 Web 安全评估工具，基于 OWASP Web 安全测试指南 (WSTG) 构建，内含专用的检查清单编辑器并支持多语言（包括支持从右到左排版的波斯语和阿拉伯语）。

---

## 核心功能 (Key Features)

- **100% 离线与安全架构**：无需后端服务器或外部数据库；所有数据均在浏览器本地 (`localStorage`) 进行处理和存储。
- **完全多语言支持 (i18n)**：支持 7 种语言 (`fa`, `en`, `zh`, `ru`, `la`, `hi`, `ar`)，并为波斯语和阿拉伯语提供自动 RTL 布局切换。
- **全面的标准检查清单**：包含 10 个核心 OWASP 类别以及 248 多个带有 WSTG 代码和 CWE 映射的结构化安全测试。
- **高级报告生成**：通过 JSON 格式导入/导出评估数据，并提供专针对失败测试的专业 Word (`.doc`) 报告生成器（包含 POC 截图和备注）。
- **凭证管理 (POC)**：支持拖放漏洞截图，并高效存储为 Base64 格式。
- **专用检查清单编辑器 (`editor.html`)**：一个独立的编辑器，用于添加、编辑、启用/禁用测试并更新主 `checklist.json` 数据文件。

---

## 项目结构 (Project Structure)

本项目包含三个主要文件：

- `index.html` : 用于执行安全评估的主应用程序
- `editor.html` : 用于管理和编辑检查清单的图形化编辑器
- `checklist.json` : 主参考数据文件（包含 10 个类别中的 248 个测试，支持 7 种语言）

---

## 快速开始 (Getting Started)

本项目无需任何编译器、包管理器（如 NPM）或本地服务器。

1. 克隆仓库或下载文件：
   `git clone https://github.com/your-username/owasp-wstg-assessment.git`
2. 在任意现代浏览器中打开 `index.html` 即可开始安全评估。
3. 若要编辑或添加新测试，请在浏览器中打开 `editor.html`，完成修改后下载并替换更新后的 `checklist.json` 文件。

---

## 技术规格 (`checklist.json`)

- 类别数量：10 个部分（符合 Web 评估标准）
- 测试总数：248 个结构化安全测试
- 测试字段：包含 ID、WSTG 代码、严重程度（Critical, High, Medium, Low）、描述、测试目标、示例载荷以及修复建议（Remediation）。

---

## 作者 (Author)

设计与开发：**Mohammad Javad Joshani (MR.MTwoJ)**

---

## 许可证 (License)

本项目采用 **MIT License** 开源许可证。
