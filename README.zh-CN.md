<p align="center">
  <a href="README.md"><img src="https://img.shields.io/badge/English-0969da?style=flat-square" alt="English"></a>
  <a href="README.zh-CN.md"><img src="https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-c8102e?style=flat-square" alt="简体中文"></a>
  <a href="README.ja.md"><img src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E-8250df?style=flat-square" alt="日本語"></a>
</p>

# Python 基础练习

包含 100 个编号脚本和九份中文参考文档的 Python 入门学习归档。

![最近提交](https://img.shields.io/github/last-commit/NextWeb4/Python-Basic?style=flat-square)
![仓库大小](https://img.shields.io/github/repo-size/NextWeb4/Python-Basic?style=flat-square)
![GitHub 星标](https://img.shields.io/github/stars/NextWeb4/Python-Basic?style=flat-square)
![Python](https://img.shields.io/badge/Python-practice-3776AB?style=flat-square&logo=python&logoColor=white)

## 归档范围

本仓库保存早期学习序列，不是可安装的 Python 包。每个编号脚本都是具有独立假设、输入、输出和副作用的教学示例；`.docx` 是参考资料，不是运行时模块。

仓库没有适用于全部 100 个案例的受支持 Python 版本、依赖清单、虚拟环境工具、包管理器、统一入口或兼容性承诺。

## 审计清单

刷新后的默认分支树包含 **1 个目录中的 113 个文件**：

| 格式 | 数量 | 用途 |
| --- | ---: | --- |
| `.py` | 100 个 | `Python100Cases-master/001.py` 至 `100.py` |
| `.docx` | 9 个 | 语法、库、练习、ELIZA、爬虫主题和案例参考文档 |
| `.md` | 4 个 | 根目录三语 README 与仓库说明 |

目录树中没有图片资源、依赖锁文件、测试目录、Notebook、打包配置或 CI 工作流。

## 练习导览

| 范围 | 代表性主题 |
| --- | --- |
| `001.py` 至 `020.py` | 循环、算术、日期、字符串、数列、素数和因式分解 |
| `021.py` 至 `040.py` | 递归、数字题、列表操作、排序和矩阵 |
| `041.py` 至 `055.py` | 类、作用域、函数、随机数和位运算 |
| `056.py` 至 `065.py` | 绘图与 GUI 类示例 |
| `066.py` 至 `090.py` | 列表、队列、链式结构、字符串、字典和小型题目 |
| `091.py` 至 `100.py` | 时间、日期解析、文本处理和文件输入输出 |

这些范围只用于导航，不保证难度持续递增，也不代表当前最佳实践。

## 仓库导览

| 路径 | 内容与边界 |
| --- | --- |
| `Python100Cases-master/` | 100 个相互独立的编号脚本 |
| `100题.docx` | 与编号案例集相关的参考资料 |
| `python基础(1).docx` 至 `python基础(4).docx`、`Python基础语法.docx` | Python 入门学习文档 |
| `Python库.docx` | Python 库相关参考资料 |
| `ELIZA .docx` | ELIZA 相关学习文档 |
| `爬虫网易云.docx` | 网易云音乐爬虫主题文档 |

除非明确重新设计并记录资料集结构，否则不要把编号文件改成隐式共享模块。

## 历史工具要求

完整阅读所选脚本后，使用与它兼容的解释器。仓库没有确认整个资料集面向某个 Python 2 或 Python 3 版本。

已确认的兼容性例外包括已删除的 `time.clock()` API、`095.py` 对第三方 `dateutil` 的导入、需要桌面会话的 GUI 或绘图示例，以及 `097.py` 至 `099.py` 的文件写入行为。其余案例没有执行，可能还有其他要求。

## 单例安全流程

1. 选择一个编号文件，阅读导入项、输入处理、输出、循环和文件系统操作。
2. 确认解释器语法、第三方导入、GUI 要求，以及可能读取或覆盖的文件。
3. 只在可丢弃工作目录中使用合成输入运行该案例，并记录解释器版本。
4. 对照练习意图检查输出，只针对该案例记录失败或现代化选择。
5. 清理生成文件，不要把一个案例成功描述成其余 99 个案例已经验证。

仓库没有统一运行命令。检查单个案例后可能适合直接调用解释器，但不能把该命令描述为通用兼容方式。

## 兼容性与副作用

- `time.clock()` 等已删除 API 可能在当前 Python 版本中失败。
- `095.py` 需要 `dateutil`，但仓库没有依赖清单或已批准版本。
- GUI 与绘图示例可能无法在无界面会话中运行，或在不同平台表现不同。
- `097.py` 至 `099.py` 可能在当前工作目录创建或覆盖文件。
- 历史教学示例可能包含缺陷、过时写法、编码假设或不适合生产环境的行为。
- 二进制 `.docx` 可能含链接或嵌入内容，应按常规文档安全措施打开。

## 验证边界

当前未发现仓库级测试、构建、lint 或 format 命令；本次文档审计没有执行 100 个脚本中的任何一个，因此不声明某个 Python 版本完全兼容。

修改案例时，应记录输入、预期与实际输出、解释器版本、依赖版本、生成文件和清理方式。可以为该案例增加专用检查，但不能称为整个归档的测试套件。

## 维护与贡献

变更应限制在一个案例或一项有明确证据的文档修正内。保留编号文件名和示例独立性；不要为解决一个已删除 API 而批量现代化 100 个脚本，也不要静默增加依赖。

English、简体中文、日本語 README 必须保持章节顺序、数量、路径、链接、兼容性事实和副作用警告一致。

## 来源与许可证

仓库中没有许可证文件。脚本和捆绑学习文档可能来自不同来源。复制、修改或再分发代码与文档前，请确认作者和许可。

## 维护者

- HaoXiang Huang
- [didadida1688@gmail.com](mailto:didadida1688@gmail.com)
- [项目主页](https://nextweb4.github.io/)
