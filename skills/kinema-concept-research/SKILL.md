---
name: kinema-concept-research
description: |
  系统调研一个概念是否已有实现及其当前状态，通过概念澄清、中英文关键词拆解、多来源交叉搜索、深度探索和异同分析生成研究报告。用户询问“有人做过吗”、现状、竞品、已有方案或技术方向调研时使用。
---

# Kinema Concept Research for Codex

## 执行前读取

首次使用或搜索依赖不可用时，完整读取：

1. [完整研究工作流](../../SKILL.md)
2. [环境配置](../../references/ONBOARDING.md)

## Codex 规则

- 优先使用已配置的 `searxng-search-cli`；不可用时可使用当前会话提供的官方 web/search 工具，但必须记录来源并保持交叉验证。
- 根规范中的 `web_fetch` 表示使用当前可用的页面打开/抓取能力，不假设存在名为 `web_fetch` 的固定命令。
- 默认把研究材料写入当前工作区的 `projects/research-{uuid}/`；写到工作区外必须先征得用户同意。
- 深度探索 GitHub 仓库、论文和网页时保留原始 URL，不把搜索摘要当作已验证事实。
- 所有时效性结论都标注检索日期；最终报告区分来源事实、综合判断和推断。
