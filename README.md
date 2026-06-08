# Codex Skills Notes / Codex Skill 使用笔记

English | [中文](#中文)

## English

This repository documents Codex/agent skills and related resources I want to track. Each entry includes a short summary, the original source link, installation notes, and basic usage guidance.

### Skill Index

| Skill | Summary | Details |
| --- | --- | --- |
| openai/skills | Official OpenAI skill catalog for Codex, including system, curated, and experimental skills. | [View details](#openaiskills) |
| forrest-orr/artifacts-kit | Security research tool for generating Windows memory artifacts; not a Codex skill. | [View details](#forrest-orrartifacts-kit) |
| greensock/gsap-skills | Official GSAP skills for teaching agents animation APIs, timelines, ScrollTrigger, plugins, and framework usage. | [View details](#greensockgsap-skills) |
| pbakaus/impeccable | Frontend design skill and command system for higher-quality UI review, polish, motion, copy, and responsive design. | [View details](#pbakausimpeccable) |
| Leonxlnx/taste-skill | Anti-generic frontend design skills plus image-generation skills for stronger layout, typography, motion, and spacing. | [View details](#leonxlnxtaste-skill) |
| jnMetaCode/superpowers-zh | Chinese enhanced Superpowers skill set for disciplined AI coding workflows, TDD, debugging, review, and planning. | [View details](#jnmetacodesuperpowers-zh) |
| jnMetaCode/agency-agents-zh | Chinese community edition of Agency Agents with 200+ specialist AI roles across engineering, design, marketing, product, and China-specific domains. | [View details](#jnmetacodeagency-agents-zh) |
| msitarzewski/agency-agents | English Agency Agents collection: specialist AI roles with identities, workflows, deliverables, and activation guidance. | [View details](#msitarzewskiagency-agents) |

### openai/skills

#### Original Link

- Source: <https://github.com/openai/skills>

#### Install In Codex

System skills are bundled with current Codex releases. For curated or experimental skills, use Codex's skill installer:

```text
$skill-installer gh-address-comments
$skill-installer install https://github.com/openai/skills/tree/main/skills/.experimental/create-plan
```

Restart Codex after installation so the new skills are discovered.

#### How To Use

- Use this as the first place to look for official Codex skills.
- Install individual curated or experimental skills when a workflow needs repeatable instructions, scripts, or references.
- Treat each skill folder as the source of truth for its `SKILL.md`, license, and supporting files.

### forrest-orr/artifacts-kit

#### Original Link

- Source: <https://github.com/forrest-orr/artifacts-kit>

#### Install In Codex

This is not a Codex skill and should not be installed as one. Keep it as a separate security research reference.

#### How To Use

- Use only in an authorized lab or malware-analysis training environment.
- The repository is useful for understanding pseudo-malicious Windows memory artifacts and detection/testing scenarios.
- Do not mix it into normal Codex skill folders; document it separately because its purpose and risk profile are different from agent instruction skills.

### greensock/gsap-skills

#### Original Link

- Source: <https://github.com/greensock/gsap-skills>

#### Install In Codex

```powershell
npx skills add https://github.com/greensock/gsap-skills
```

Manual install option: copy the repository's `skills/` folders into `~/.codex/skills/`, then restart Codex.

#### How To Use

- Use when building JavaScript animation with GSAP in React, Vue, Svelte, or vanilla JS.
- Good for timelines, staggered animation, ScrollTrigger, MotionPath, Flip, plugin usage, cleanup, and performance.
- Especially helpful when the agent might otherwise generate fragile animation code or misuse framework lifecycles.

### pbakaus/impeccable

#### Original Link

- Source: <https://github.com/pbakaus/impeccable>

#### Install In Codex

Recommended installer:

```powershell
npx impeccable skills install
```

Repository-based install option:

```powershell
git submodule add https://github.com/pbakaus/impeccable .impeccable
npx impeccable skills link --source=.impeccable --providers=codex
```

#### How To Use

- Use for frontend design critique, polishing, responsive hardening, UX copy, animation, and visual quality checks.
- Commands include `/impeccable audit`, `/impeccable critique`, `/impeccable polish`, `/impeccable harden`, `/impeccable animate`, and more.
- Best used after a UI exists or before building a high-polish interface that needs a strong design language.

### Leonxlnx/taste-skill

#### Original Link

- Source: <https://github.com/Leonxlnx/taste-skill>

#### Install In Codex

Install all skills:

```powershell
npx skills add https://github.com/Leonxlnx/taste-skill
```

Install only the default frontend taste skill:

```powershell
npx skills add https://github.com/Leonxlnx/taste-skill --skill "design-taste-frontend"
```

#### How To Use

- Use when AI-generated UI feels generic, under-designed, or visually flat.
- Pick a specific skill for the job: `design-taste-frontend`, `gpt-taste`, `image-to-code`, `redesign-existing-projects`, `high-end-visual-design`, `minimalist-ui`, or `industrial-brutalist-ui`.
- Use its image-generation skills for web comps, mobile flows, or brand boards before implementing with Codex.

### jnMetaCode/superpowers-zh

#### Original Link

- Source: <https://github.com/jnMetaCode/superpowers-zh>

#### Install In Codex

```powershell
npx superpowers-zh
```

If auto-detection does not find Codex, specify the tool:

```powershell
npx superpowers-zh --tool codex
```

#### How To Use

- Use when you want AI coding to follow structured workflows: brainstorming, planning, TDD, debugging, code review, worktrees, and verification before completion.
- Good for Chinese-language teams because it keeps technical terms readable while adapting communication, Git workflow, commit conventions, and documentation style.
- Also includes China-specific skills such as Chinese code review, Chinese Git workflow, Chinese documentation, Chinese commit conventions, MCP builder, and workflow runner.

### jnMetaCode/agency-agents-zh

#### Original Link

- Source: <https://github.com/jnMetaCode/agency-agents-zh>

#### Install In Codex

From the cloned repository, run with Git Bash, WSL, or another shell that supports `.sh` scripts:

```bash
./scripts/install.sh --tool codex
```

#### How To Use

- Use when you want named specialist roles rather than general-purpose prompts.
- Useful roles cover engineering, design, product, marketing, finance, legal, support, testing, game development, and China-market scenarios such as Xiaohongshu, Douyin, WeChat, Feishu, DingTalk, cross-border ecommerce, and compliance.
- Activate an agent by asking Codex to use the relevant specialist role for the task.

### msitarzewski/agency-agents

#### Original Link

- Source: <https://github.com/msitarzewski/agency-agents>

#### Install In Codex

From the cloned repository:

```bash
./scripts/convert.sh
./scripts/install.sh --tool codex
```

#### How To Use

- Use as a library of English specialist AI roles.
- Each agent file includes identity, mission, workflow, deliverables, success metrics, and communication style.
- Good when a task benefits from a named expert persona, such as frontend developer, security reviewer, product strategist, QA tester, or marketing specialist.

---

## 中文

这个仓库用于维护我在使用 Codex / AI Agent 过程中关注的 skills 和相关资源。每个条目包含简介、原文链接、如何安装到 Codex，以及如何使用。

### Skill 索引

| Skill 名字 | 简介 | 详情链接 |
| --- | --- | --- |
| openai/skills | OpenAI 官方 Codex skill 目录，包含系统、精选和实验性 skills。 | [查看详情](#openaiskills-1) |
| forrest-orr/artifacts-kit | Windows 内存伪迹生成的安全研究工具；不是 Codex skill。 | [查看详情](#forrest-orrartifacts-kit-1) |
| greensock/gsap-skills | GSAP 官方 AI skills，用于动画 API、时间线、ScrollTrigger、插件和框架实践。 | [查看详情](#greensockgsap-skills-1) |
| pbakaus/impeccable | 前端设计质量 skill 和命令系统，用于 UI 审查、打磨、动效、文案和响应式设计。 | [查看详情](#pbakausimpeccable-1) |
| Leonxlnx/taste-skill | 反模板化前端设计 skills，并包含用于参考图、移动端、品牌板的图像生成 skills。 | [查看详情](#leonxlnxtaste-skill-1) |
| jnMetaCode/superpowers-zh | 中文增强版 Superpowers，覆盖需求澄清、计划、TDD、调试、代码审查和完成前验证。 | [查看详情](#jnmetacodesuperpowers-zh-1) |
| jnMetaCode/agency-agents-zh | 中文社区版 AI 专家角色库，覆盖工程、设计、营销、产品以及中国市场垂直场景。 | [查看详情](#jnmetacodeagency-agents-zh-1) |
| msitarzewski/agency-agents | 英文版 AI 专家角色库，每个 agent 有身份、流程、交付物和调用方式。 | [查看详情](#msitarzewskiagency-agents-1) |

### openai/skills

#### 原文链接

- 原文：<https://github.com/openai/skills>

#### 如何安装到 Codex

系统 skills 会随新版 Codex 自动安装。精选或实验性 skills 可以用 Codex 的 skill installer：

```text
$skill-installer gh-address-comments
$skill-installer install https://github.com/openai/skills/tree/main/skills/.experimental/create-plan
```

安装后重启 Codex，让新 skill 被识别。

#### 如何使用

- 把它作为查找官方 Codex skills 的首选入口。
- 当某个工作流需要可重复的方法、脚本或参考资料时，安装对应的精选或实验性 skill。
- 每个 skill 目录里的 `SKILL.md`、许可证和附属文件应作为原始依据。

### forrest-orr/artifacts-kit

#### 原文链接

- 原文：<https://github.com/forrest-orr/artifacts-kit>

#### 如何安装到 Codex

这不是 Codex skill，不建议安装进 Codex skills 目录。它更适合作为独立的安全研究资料保存。

#### 如何使用

- 只在授权的安全实验室、恶意样本分析训练或检测规则测试环境中使用。
- 可用于理解 Windows 内存伪迹、检测场景和安全研究中的模拟痕迹。
- 不要把它和普通 Codex skill 混在一起维护，因为它的用途和风险级别完全不同。

### greensock/gsap-skills

#### 原文链接

- 原文：<https://github.com/greensock/gsap-skills>

#### 如何安装到 Codex

```powershell
npx skills add https://github.com/greensock/gsap-skills
```

手动安装方式：把仓库里的 `skills/` 目录复制到 `~/.codex/skills/`，然后重启 Codex。

#### 如何使用

- 在 React、Vue、Svelte 或原生 JS 中做 GSAP 动画时使用。
- 适合时间线、交错动画、ScrollTrigger、MotionPath、Flip、插件注册、清理和性能优化。
- 当 AI 容易写出脆弱动画代码或误用框架生命周期时，这个 skill 很有价值。

### pbakaus/impeccable

#### 原文链接

- 原文：<https://github.com/pbakaus/impeccable>

#### 如何安装到 Codex

推荐安装方式：

```powershell
npx impeccable skills install
```

通过 Git 子模块安装：

```powershell
git submodule add https://github.com/pbakaus/impeccable .impeccable
npx impeccable skills link --source=.impeccable --providers=codex
```

#### 如何使用

- 用于前端设计审查、视觉打磨、响应式加固、UX 文案、动效和最终质量检查。
- 常用命令包括 `/impeccable audit`、`/impeccable critique`、`/impeccable polish`、`/impeccable harden`、`/impeccable animate` 等。
- 适合已有 UI 后做质量提升，也适合高要求界面开发前先建立设计语言。

### Leonxlnx/taste-skill

#### 原文链接

- 原文：<https://github.com/Leonxlnx/taste-skill>

#### 如何安装到 Codex

安装全部 skills：

```powershell
npx skills add https://github.com/Leonxlnx/taste-skill
```

只安装默认前端审美 skill：

```powershell
npx skills add https://github.com/Leonxlnx/taste-skill --skill "design-taste-frontend"
```

#### 如何使用

- 当 AI 生成的 UI 显得模板化、廉价、无设计感时使用。
- 可按任务选择 `design-taste-frontend`、`gpt-taste`、`image-to-code`、`redesign-existing-projects`、`high-end-visual-design`、`minimalist-ui`、`industrial-brutalist-ui` 等。
- 也可以使用其中的图像生成 skills，先生成网站稿、移动端流程或品牌板，再交给 Codex 实现。

### jnMetaCode/superpowers-zh

#### 原文链接

- 原文：<https://github.com/jnMetaCode/superpowers-zh>

#### 如何安装到 Codex

```powershell
npx superpowers-zh
```

如果自动检测不到 Codex，可以显式指定：

```powershell
npx superpowers-zh --tool codex
```

#### 如何使用

- 当你希望 AI 编程严格遵循结构化方法时使用：头脑风暴、计划、TDD、系统化调试、代码审查、worktree 和完成前验证。
- 适合中文团队，技术术语保留英文，同时适配国内沟通方式、Git 工作流、提交规范和中文文档风格。
- 还包含中文代码审查、中文 Git 工作流、中文技术文档、中文提交规范、MCP 服务器构建和工作流执行器等中国特色 skills。

### jnMetaCode/agency-agents-zh

#### 原文链接

- 原文：<https://github.com/jnMetaCode/agency-agents-zh>

#### 如何安装到 Codex

克隆仓库后，在 Git Bash、WSL 或其他支持 `.sh` 的 shell 中运行：

```bash
./scripts/install.sh --tool codex
```

#### 如何使用

- 当你希望 Codex 调用“专家角色”而不是普通提示词时使用。
- 角色覆盖工程、设计、产品、营销、金融、法务、支持、测试、游戏开发，以及小红书、抖音、微信、飞书、钉钉、跨境电商和合规等中国市场场景。
- 使用时直接让 Codex 激活对应专家角色来处理任务。

### msitarzewski/agency-agents

#### 原文链接

- 原文：<https://github.com/msitarzewski/agency-agents>

#### 如何安装到 Codex

克隆仓库后运行：

```bash
./scripts/convert.sh
./scripts/install.sh --tool codex
```

#### 如何使用

- 作为英文 AI 专家角色库使用。
- 每个 agent 文件包含身份、使命、工作流程、交付物、成功指标和沟通风格。
- 适合需要专家人设的任务，例如前端开发、安全审查、产品策略、QA 测试或营销策略。
