# Agent Skill 共享规则 / Agent Skill Sharing Rules

> 公开分享版，已移除本机路径、账号标识和其他可识别个人隐私。
>
> Public sharing version with local paths, account identifiers, and other personally identifiable information removed.

## 中文版

### 1. 可共享的 Skill
- 只有包含 `SKILL.md` 的 portable skill 才能直接共享。
- 插件、MCP、App 不是直接可共享的 skill 形态，需要先说明边界，再决定是否做 wrapper。
- 共享内容应尽量保留通用逻辑，避免绑定某台机器或某个账号。

### 2. 共享源与归属
- 共享 skill 的 canonical 源应集中在统一位置管理。
- 只修改 canonical 源，不把本地生成物、缓存目录或个人工作区当成最终来源。
- 如果存在 overlay 形态，只共享通用代码；本机私有配置保持本地化。

### 3. 隐私保护
- 不要硬编码密钥、token、密码或连接字符串。
- 不要公开本机用户名、绝对路径、私有域名、账号标识或内部服务地址。
- 示例路径应抽象化，例如使用 `<workspace>`、`<skill-root>` 之类的占位符。
- 日志、注释和 README 中也不要泄露敏感信息。

### 4. 推荐更新流程
1. 先编辑共享源。
2. 再做只读审计，确认共享 / 本地 / overlay 的边界正确。
3. 然后执行分发或重建步骤。
4. 最后做语法和一致性校验，确认没有引入脏生成物。

### 5. 质量要求
- 变更前先判断是否会影响现有共享规则。
- 变更后必须验证，不要在未验证时声称成功。
- 如果需要删除或重命名现有文件，先征得确认。

### 6. 一句话版
- 先改共享源，再做审计，再分发，再验证。
- 只共享通用能力，不共享个人环境。

## English

### 1. What can be shared
- Only portable skills with a `SKILL.md` file are directly shareable.
- Plugins, MCP tools, and apps are not directly shareable skill formats; first clarify the boundary, then decide whether a wrapper is needed.
- Shared content should stay generic and avoid binding to one machine or one account.

### 2. Source of truth
- Keep the canonical source of a shared skill in one shared location.
- Update only the canonical source, and do not treat local build outputs, caches, or personal workspaces as the source of truth.
- If an overlay exists, share only common code; keep machine-specific settings local.

### 3. Privacy protection
- Do not hard-code secrets, tokens, passwords, or connection strings.
- Do not expose local usernames, absolute paths, private domains, account identifiers, or internal service endpoints.
- Abstract example paths with placeholders such as `<workspace>` or `<skill-root>`.
- Avoid leaking sensitive data in logs, comments, or README files.

### 4. Recommended update flow
1. Edit the shared source first.
2. Run a read-only audit to verify shared, local, and overlay boundaries.
3. Run the distribution or rebuild step.
4. Finish with syntax and consistency checks to avoid dirty generated artifacts.

### 5. Quality bar
- Check whether a change affects existing sharing rules before editing.
- Verify after the change; do not claim success without validation.
- If deleting or renaming existing files, ask first.

### 6. One-line version
- Edit the shared source, audit it, distribute it, then verify it.
- Share common capability only, not personal environment details.
