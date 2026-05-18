---
name: 'prompt-optimizer'
description: '分析原始提示，识别意图和差距，匹配ECC组件（技能/命令/代理/钩子），并输出一个可直接粘贴的优化提示。仅提供咨询角色——绝不自行执行任务。触发时机：当用户说“优化提示”、“改进我的提示”、“如何编写提示”、“帮我优化这个指令”或明确要求提高提示质量时。中文等效表达同样触发：“优化prompt”、“改进prompt”、“怎么写prompt”、“帮我优化这个指令”。不触发时机：当用户希望直接执行任务'
adopted: 2026-05-16
batch: bulk-adoption
source: everything-claude-code
tier: 3
version: 1.0.0
---

# prompt-optimizer

分析原始提示，识别意图和差距，匹配ECC组件（技能/命令/代理/钩子），并输出一个可直接粘贴的优化提示。仅提供咨询角色——绝不自行执行任务。触发时机：当用户说“优化提示”、“改进我的提示”、“如何编写提示”、“帮我优化这个指令”或明确要求提高提示质量时。中文等效表达同样触发：“优化prompt”、“改进prompt”、“怎么写prompt”、“帮我优化这个指令”。不触发时机：当用户希望直接执行任务

## When to Use

- Use this skill when working on tasks related to prompt optimizer
- Apply best practices from everything-claude-code

## Workflow

name: prompt-optimizer
description: 分析原始提示，识别意图和差距，匹配ECC组件（技能/命令/代理/钩子），并输出一个可直接粘贴的优化提示。仅提供咨询角色——绝不自行执行任务。触发时机：当用户说“优化提示”、“改进我的提示”、“如何编写提示”、“帮我优化这个指令”或明确要求提高提示质量时。中文等效表达同样触发：“优化prompt”、“改进prompt”、“怎么写prompt”、“帮我优化这个指令”。不触发时机：当用户希望直接执行任务，或说“直接做”时。不触发时机：当用户说“优化代码”、“优化性能”、“optimize performance”、“optimize this code”时——这些是重构/性能优化任务，而非提示优化。
origin: community
metadata:
  author: YannJY02
  version: "1.0.0"
# Prompt 优化器
分析一个草稿提示，对其进行评估，匹配到 ECC 生态系统组件，并输出一个完整的优化提示供用户复制粘贴并运行。
## 何时使用
* 用户说“优化这个提示”、“改进我的提示”、“重写这个提示”
* 用户说“帮我写一个更好的提示来...”
* 用户说“询问 Claude Code 的...最佳方式是什么？”
* 用户说“优化prompt”、“改进prompt”、“怎么写p

## Source

Adopted from: everything-claude-code
