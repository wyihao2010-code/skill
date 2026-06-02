# Agent Skill 共享规则

> 仅供公开参考。已移除本机路径、账号标识和其他可识别个人隐私信息。

## 目的

本仓库用于沉淀一套可复用的 agent skill 共享规则，适用于跨环境共享，同时避免在公开文档中暴露敏感信息。

## 适用范围

- 带有 `SKILL.md` 的 portable skill
- 共享 skill 的分发与同步
- 面向公开仓库的共享规则文档
- 经过脱敏处理的示例与流程说明

## 核心原则

1. 只共享可移植、通用的能力。
2. 将 canonical 源集中在统一位置管理。
3. 本地生成物、缓存目录和个人工作区不作为权威来源。
4. 使用 overlay 模式时，仅共享通用代码，本机私有配置保持本地化。
5. 不发布密钥、token、密码、连接字符串或内部服务地址。
6. 使用 `<workspace>`、`<skill-root>` 等占位符替代具体路径和标识。

## 推荐流程

1. 编辑共享源。
2. 执行只读审计，确认共享 / 本地 / overlay 的边界。
3. 按需执行分发或重建步骤。
4. 在发布或同步前完成语法与一致性校验。

## 质量要求

- 变更后必须验证，未验证前不宣称成功。
- 删除或重命名现有文件前先确认。
- 文档中不得出现敏感信息。
- 优先使用简短、明确的规则，避免模糊表达。

## 如何使用

### 查询

- 按仓库名搜索：`wyihao2010-code/skill`
- 按主题搜索：`Agent Skill Sharing Rules`
- 按关键词搜索：`portable skill`、`SKILL.md`、`overlay`、`canonical source`、`privacy-safe`

### 使用

1. 先阅读仓库总览。
2. 判断对应 skill 是否可移植、可共享。
3. 只修改共享内容的 canonical 源。
4. 本机私有配置保持本地化。
5. 发布前移除密钥、私有路径和其他可识别信息。

### 引用

- 可将本仓库作为 agent skill 共享规则模板。
- 复制、改写或再分发时请保留署名。
- 遵循 `LICENSE` 中的许可条款。

## 一句话总结

先改共享源，再审计，再分发，最后验证。

---

# Agent Skill Sharing Rules

> Public reference only. Local paths, account identifiers, and other personally identifiable information have been removed.

## Purpose

This repository captures a reusable rule set for sharing agent skills across environments while keeping sensitive information out of public documentation.

## Scope

- Portable skills with a `SKILL.md` file
- Shared skill distribution and synchronization
- Public-facing documentation for sharing rules
- Privacy-safe examples and process notes

## Core Principles

1. Share only portable, generic capability.
2. Keep the canonical source in one shared location.
3. Treat local build outputs, caches, and personal workspaces as non-authoritative.
4. Keep machine-specific settings local when overlay patterns are used.
5. Never publish secrets, tokens, passwords, connection strings, or internal endpoints.
6. Replace concrete paths and identifiers with placeholders such as `<workspace>` and `<skill-root>`.

## Recommended Workflow

1. Edit the shared source.
2. Run a read-only audit to confirm shared, local, and overlay boundaries.
3. Run distribution or rebuild steps as needed.
4. Validate syntax and consistency before publishing or syncing.

## Quality Bar

- Verify changes before claiming success.
- Ask first before deleting or renaming existing files.
- Keep documentation free of sensitive data.
- Prefer short, explicit rules over vague guidance.

## How to Use

### Find

- Search by repository name: `wyihao2010-code/skill`
- Search by topic: `Agent Skill Sharing Rules`
- Search by keywords: `portable skill`, `SKILL.md`, `overlay`, `canonical source`, `privacy-safe`

### Apply

1. Read the repository overview first.
2. Check whether the skill is portable and shareable.
3. Edit only the canonical source for shared content.
4. Keep machine-specific settings local.
5. Remove secrets, private paths, and other identifying details before publishing.

### Reference

- Use this repository as a rule template for agent skill sharing.
- Keep attribution when copying, adapting, or redistributing the content.
- Follow the license terms in `LICENSE`.

## One-Line Summary

Edit the shared source, audit it, distribute it, then verify it.
