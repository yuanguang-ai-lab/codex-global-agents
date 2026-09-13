# Codex Global AGENTS.md

面向 GPT-6 Astra 整理的通用全局工作约定。可复制并按自己的工作习惯修改；其他模型也可使用，但应观察实际效果后调整。

核心文件：[AGENTS.md](AGENTS.md)。它保留任务完成、证据判断、授权边界、适度验证、Git 安全与任务交接，减少重复审批和固定流程。

## 使用方法

1. 下载或复制本仓库的 `AGENTS.md`。
2. 如果已有全局规则，先备份并比较；把需要的约定合并进去，避免直接覆盖个人设置。
3. 将结果保存为 Codex 配置目录下的 `AGENTS.md`。默认路径是 `~/.codex/AGENTS.md`；如果配置了 `CODEX_HOME`，使用该目录。
4. 检查是否存在优先加载的 `AGENTS.override.md`，然后在新任务中确认实际使用了预期规则。保留 override 的用途，不要为了安装本模板盲目删除它。

文件名应为 **`AGENTS.md`**。项目根目录也可以放同名文件，补充该项目的命令、目录边界、验证方式与约束；不必重复整份全局约定。[官方加载规则](https://learn.chatgpt.com/docs/agent-configuration/agents-md)

## 按需调整

- 语言和回复长度：模板跟随当前用户，不预设中文或英文。
- GitHub 授权：模板本身不授权推送、创建 PR 或发布；以实际用户请求和仓库权限为准。
- 交接目录：`.codex/handoffs/` 是可采用的约定；已有项目结构时按项目规则处理。
- 代理、技能和计划任务：仅使用当前环境具备且任务需要的能力。
- 项目规则：增加真实的本地约束和已核实命令，不把每个临时问题写成永久规则。

本文件是行为指导，不会修改模型、账户权限、审批策略、插件或运行环境，也没有实现“新建项目时自动生成局部规则”的自动化。

## 脱敏范围

当前版本已移除个人用户名、固定机器路径、个人账号的预授权和专属语言偏好。只提供通用模板和说明，不包含个人配置、凭据、记忆、会话、日志或本地备份。

**这里的脱敏声明仅覆盖当前文件内容。早期提交保留了历史配置，不属于脱敏版本；如需分享，请优先复制当前 `AGENTS.md`。更改仓库可见性前应单独审查历史。**

## 修改依据

- [OpenAI GPT-6 Astra Model Guidance](https://developers.openai.com/api/docs/guides/latest-model?model=gpt-6-astra)
- [Eric Provencher: Rethinking skills and prompts for GPT-6 Astra](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra)

这是个人整理的可复用模板，不是 OpenAI 官方默认配置。精简目标是减少无用约束，不能据此承诺固定的 Token 节省或跨任务效果。
