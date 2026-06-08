# Codex Skills Notes / Codex Skill 使用笔记

中文 | [English](#english)

### Skill Store 资源入口

[Skillstore - Codex code review skills](https://skillstore.io/zh-hans/skills?q=code+review&tools=codex) 是一个面向 AI Agent skills 的检索网站。这个页面已经筛选了 `code review` 关键词和 `Codex` 工具，可以快速查看适用于 Codex 的代码审查相关 skills，包括请求代码审查、处理审查反馈、PR 工作流、安全与质量检查、多代理审查等方向。适合在需要寻找新的代码审查 skill 或比较同类 skill 时作为入口。

### 当前 Codex 环境中的内置/插件 Skills

下面这些是当前本机 Codex 环境扫描到的 skills，主要来自两个位置：

- 本地 skills：`C:\Users\admin\.codex\skills`
- 插件缓存 skills：`C:\Users\admin\.codex\plugins\cache`

这些条目大多是 Codex 自带或当前已启用插件提供的能力，并不是独立的外部 GitHub skill 仓库。没有独立原文链接的条目，原文链接位置统一说明为“当前 Codex 本地环境或插件缓存，暂无独立原文链接”。

#### 本地安装 / 系统 Skills

| 来源 | Skills | 原文链接说明 | 简介 |
| --- | --- | --- | --- |
| local / system | `imagegen` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 生成或编辑图片、纹理、插画、mockup 等位图视觉资产。 |
| local / system | `openai-docs` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 查询 OpenAI / Codex 官方产品和 API 文档时使用。 |
| local / system | `plugin-creator` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 创建或维护 Codex 插件目录和 manifest。 |
| local / system | `skill-creator` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 创建或更新 Codex skills 的工作流指导。 |
| local / system | `skill-installer` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 从精选列表或 GitHub 仓库安装 Codex skills。 |
| local | `pdf` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 读取、创建、审阅 PDF，尤其适合需要渲染校验的场景。 |
| local | `playwright` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 使用真实浏览器自动化测试、截图、调试页面流程。 |

#### 插件 Skills

| 插件 / 来源 | Skills | 原文链接说明 | 简介 |
| --- | --- | --- | --- |
| Browser | `control-in-app-browser` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 控制 Codex 内置浏览器，打开、检查、点击和截图本地或网页目标。 |
| Chrome | `chrome` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 控制用户 Chrome 浏览器，适合需要登录态、扩展或现有标签页的任务；当前缓存里有两个版本。 |
| Computer Use | `computer-use` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 控制 Windows 桌面应用。 |
| Documents | `documents` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 创建、编辑、渲染和校验 Word / docx 文档。 |
| Presentations | `presentations` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 创建、编辑和验证 PPTX / 演示文稿。 |
| Spreadsheets | `spreadsheets` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 创建、编辑、分析、可视化电子表格。 |
| GitHub | `github`, `gh-address-comments`, `gh-fix-ci`, `yeet` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | GitHub 仓库、PR、Issue、代码审查反馈、CI 修复、提交推送和 PR 创建工作流。 |
| Figma | `figma-code-connect`, `figma-create-new-file`, `figma-generate-design`, `figma-generate-diagram`, `figma-generate-library`, `figma-use`, `figma-use-figjam`, `figma-use-slides` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | Figma 文件创建、设计生成、图表生成、组件库、变量、FigJam 和 Slides 操作。 |
| Netlify | `netlify-ai-gateway`, `netlify-blobs`, `netlify-caching`, `netlify-cli-and-deploy`, `netlify-config`, `netlify-deploy`, `netlify-edge-functions`, `netlify-forms`, `netlify-frameworks`, `netlify-functions`, `netlify-identity`, `netlify-image-cdn` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | Netlify 部署、配置、函数、表单、边缘函数、缓存、身份认证、图片 CDN 和 AI Gateway。 |
| Superpowers | `brainstorming`, `dispatching-parallel-agents`, `executing-plans`, `finishing-a-development-branch`, `receiving-code-review`, `requesting-code-review`, `subagent-driven-development`, `systematic-debugging`, `test-driven-development`, `using-git-worktrees`, `using-superpowers`, `verification-before-completion`, `writing-plans`, `writing-skills` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 结构化 AI 编程流程，包括计划、TDD、调试、代码审查、worktree、并行 agent 和完成前验证。 |
| Codex Context Ops | `context-agency-agents-install`, `context-bug-memory`, `context-feature-index`, `context-governance`, `context-init`, `context-release-check`, `context-safe-bugfix`, `context-safe-refactor`, `context-safe-review`, `context-subagents`, `context-worktree` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 管理上下文、索引功能、安装 agents、执行安全 bugfix / refactor / review、worktree 和发布检查。 |
| Sales | `analyze-account-signals`, `build-business-case`, `build-competitive-brief`, `enrich-company-and-contact-data`, `find-customer-quotes`, `find-key-internal-sources`, `follow-up-after-call`, `get-rep-call-feedback`, `hubspot`, `index`, `plan-deal-strategy`, `prepare-for-meeting`, `prioritize-accounts`, `review-forecast`, `review-rep-call-trends`, `sales-company-research`, `salesforce`, `suggest-sales-next-step`, `user-context`, `zoominfo` | 当前 Codex 本地环境或插件缓存，暂无独立原文链接。 | 销售场景工作流，包括会议准备、通话跟进、客户研究、预测审查、竞品简报、CRM 和联系人数据增强。 |

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

#### 详细说明

`openai/skills` 是 OpenAI 官方的 Codex skill 目录。Skill 本质上是一个包含说明、脚本和参考资料的文件夹，Codex 可以在任务匹配时加载它。它的价值在于把可复用的工作方法从一次性 prompt 中抽离出来：同样的流程不需要每次重新解释，安装一次后 Codex 就可以按需发现和使用。

这个仓库包含 Codex 自带的系统 skills、常见工作流的精选 skills，以及较新的实验性 skills。它也适合作为学习资料，用来理解一个标准 `SKILL.md` 应该怎么写、skill 目录如何组织、脚本和参考资料如何一起打包。

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

#### 详细说明

`forrest-orr/artifacts-kit` 不是 AI Agent skill，而是一个 Windows 安全研究工具。它可以生成类似恶意软件行为的用户态内存伪迹，供安全分析师研究、演示或测试检测规则。它关注的是内存分配、载荷映射、执行方式和隐蔽痕迹，因此适合防御研究，不适合作为 Codex skill 安装。

在这个文档中，它应该被归类为相关安全资料，而不是 Codex 技能。重点是保持隔离：不要放入 `~/.codex/skills/`，不要当作 agent 指令包使用，也只应在授权、受控的安全实验环境中运行。

#### 如何安装到 Codex

这不是 Codex skill，不建议安装进 Codex skills 目录。它更适合作为独立的安全研究资料保存。

#### 如何使用

- 只在授权的安全实验室、恶意样本分析训练或检测规则测试环境中使用。
- 可用于理解 Windows 内存伪迹、检测场景和安全研究中的模拟痕迹。
- 不要把它和普通 Codex skill 混在一起维护，因为它的用途和风险级别完全不同。

### greensock/gsap-skills

#### 原文链接

- 原文：<https://github.com/greensock/gsap-skills>

#### 详细说明

`greensock/gsap-skills` 是 GSAP 官方的 Agent Skills 包。GSAP 是 GreenSock Animation Platform，这组 skills 会教 AI 正确使用 GSAP API，包括基础 tween、timeline、ScrollTrigger、插件、工具函数、框架生命周期清理，以及动画性能相关实践。

动画代码很容易出现细节问题，例如忘记注册插件、React effect 清理不完整、选择器作用域泄漏、滚动动画没有刷新布局、使用低性能布局属性等。这个 skill 可以让 Codex 在 React、Vue、Svelte 或原生 JavaScript 项目中生成更稳定、可维护的 GSAP 动画代码。

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

#### 详细说明

`pbakaus/impeccable` 是一个前端设计 skill 系统，用来提升 AI 的视觉判断和产品设计表达。它不只是一个简单风格指南，而是包含设计 skill、字体、颜色、空间、动效、交互、响应式和 UX 文案等参考资料，并提供 audit、critique、polish、harden、animate、layout、clarify 等命令式工作流。

它的核心价值是帮助 AI 避免常见的模板化 UI 和廉价视觉套路，让界面设计更有判断力。适合用于高质量前端项目、设计系统对齐、响应式检查、可访问性检查、文案优化，以及上线前的最终视觉打磨。

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

#### 详细说明

`Leonxlnx/taste-skill` 是一组用于提升 AI 前端审美的可移植 agent skills。默认 skill 会强调更好的布局、字体、间距、动效和设计语言推断，避免生成看起来像模板的普通界面。它还包含面向 GPT/Codex 的更严格版本、已有项目 redesign 工作流、image-to-code 工作流，以及 minimalist、高端柔和、工业粗野等风格方向。

当问题不是代码能不能跑，而是 UI 看起来平庸、不精致、缺少设计感时，这个仓库很有用。它可以帮助 Codex 先判断设计方向，再做构图、排版、动效和视觉层次，也可以配合参考图、移动端流程图或品牌板来完成从视觉探索到代码实现的过程。

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

#### 详细说明

`jnMetaCode/superpowers-zh` 是 Superpowers skill 框架的中文增强版。它把 AI 编程从“收到需求就直接写代码”变成结构化流程，包括头脑风暴、编写计划、测试驱动开发、系统化调试、请求和接收代码审查、使用 worktree 隔离开发，以及完成前必须验证。

相比英文上游版本，它增加了中文翻译、更广泛的工具支持，以及面向中国开发者的工作流。适合希望 Codex 多问关键问题、先想清楚再实现、遵守工程纪律，并且能用中文技术文档和国内团队习惯沟通的开发者。

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

#### 详细说明

`jnMetaCode/agency-agents-zh` 是 Agency Agents 的中文社区版。它不是单一工作流，而是一套大型 AI 专家角色库。每个角色都有身份、专业领域、工作流程和交付物，Codex 可以按任务切换为前端专家、产品策略师、测试专家、营销专家、法务审查、客服专家或中国市场运营角色。

这个版本在翻译英文上游角色的基础上，新增了大量中国市场相关角色，例如小红书、抖音、微信、B 站、飞书、钉钉、跨境电商、政企 ToG、合规行业等。它适合那些需要“明确专家视角”的任务，而不是只让 Codex 泛泛地回答。

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

#### 详细说明

`msitarzewski/agency-agents` 是英文版 Agency Agents 上游仓库。它像一个完整的 AI 专家团队，每个 agent 都有明确的专业身份、沟通风格、工作流程、交付物和成功指标。角色覆盖工程、设计、产品、营销、销售、金融、安全、测试、战略、支持等多个领域。

这个仓库的价值在于角色精度。与其临时要求 Codex “扮演某个专家”，不如使用已经写好的 agent 定义，让模型知道这个专家应该如何思考、按什么步骤工作，以及输出什么样的成果才算合格。

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
---


### Skill Store Entry

[Skillstore - Codex code review skills](https://skillstore.io/zh-hans/skills?q=code+review&tools=codex) is a searchable catalog for AI Agent skills. This page is filtered by the `code review` keyword and the `Codex` tool, so it is useful for quickly finding Codex-compatible skills related to code review, review feedback, PR workflows, security and quality checks, and multi-agent review. Use it as a discovery entry point when comparing or looking for new code review skills.

### Built-In And Plugin Skills In This Codex Environment

The following skills were found in the current local Codex environment. They mainly come from:

- Local skills: `C:\Users\admin\.codex\skills`
- Plugin cache skills: `C:\Users\admin\.codex\plugins\cache`

Most of these are built into Codex or provided by currently enabled plugins. They are not independent external GitHub skill repositories. When a skill has no standalone original source link, the source note says: "Current Codex local environment or plugin cache; no standalone original link."

#### Local / System Skills

| Source | Skills | Source Link Note | Summary |
| --- | --- | --- | --- |
| local / system | `imagegen` | Current Codex local environment or plugin cache; no standalone original link. | Generate or edit bitmap visual assets such as images, textures, illustrations, and mockups. |
| local / system | `openai-docs` | Current Codex local environment or plugin cache; no standalone original link. | Look up official OpenAI / Codex product and API documentation. |
| local / system | `plugin-creator` | Current Codex local environment or plugin cache; no standalone original link. | Create or maintain Codex plugin directories and manifests. |
| local / system | `skill-creator` | Current Codex local environment or plugin cache; no standalone original link. | Create or update Codex skills. |
| local / system | `skill-installer` | Current Codex local environment or plugin cache; no standalone original link. | Install Codex skills from curated lists or GitHub repositories. |
| local | `pdf` | Current Codex local environment or plugin cache; no standalone original link. | Read, create, and review PDFs, especially when rendered layout checks matter. |
| local | `playwright` | Current Codex local environment or plugin cache; no standalone original link. | Automate a real browser for tests, screenshots, and UI-flow debugging. |

#### Plugin Skills

| Plugin / Source | Skills | Source Link Note | Summary |
| --- | --- | --- | --- |
| Browser | `control-in-app-browser` | Current Codex local environment or plugin cache; no standalone original link. | Control the in-app Codex browser for opening, inspecting, clicking, and screenshotting local or web targets. |
| Chrome | `chrome` | Current Codex local environment or plugin cache; no standalone original link. | Control the user's Chrome browser for authenticated sessions, extensions, or existing tabs; two cached versions are present. |
| Computer Use | `computer-use` | Current Codex local environment or plugin cache; no standalone original link. | Control Windows desktop apps. |
| Documents | `documents` | Current Codex local environment or plugin cache; no standalone original link. | Create, edit, render, and verify Word / docx documents. |
| Presentations | `presentations` | Current Codex local environment or plugin cache; no standalone original link. | Create, edit, and verify PPTX presentations. |
| Spreadsheets | `spreadsheets` | Current Codex local environment or plugin cache; no standalone original link. | Create, edit, analyze, and visualize spreadsheets. |
| GitHub | `github`, `gh-address-comments`, `gh-fix-ci`, `yeet` | Current Codex local environment or plugin cache; no standalone original link. | GitHub repository, PR, issue, review-feedback, CI-fix, commit, push, and PR-creation workflows. |
| Figma | `figma-code-connect`, `figma-create-new-file`, `figma-generate-design`, `figma-generate-diagram`, `figma-generate-library`, `figma-use`, `figma-use-figjam`, `figma-use-slides` | Current Codex local environment or plugin cache; no standalone original link. | Figma file creation, design generation, diagram generation, component libraries, variables, FigJam, and Slides operations. |
| Netlify | `netlify-ai-gateway`, `netlify-blobs`, `netlify-caching`, `netlify-cli-and-deploy`, `netlify-config`, `netlify-deploy`, `netlify-edge-functions`, `netlify-forms`, `netlify-frameworks`, `netlify-functions`, `netlify-identity`, `netlify-image-cdn` | Current Codex local environment or plugin cache; no standalone original link. | Netlify deployment, config, functions, forms, edge functions, caching, identity, Image CDN, and AI Gateway workflows. |
| Superpowers | `brainstorming`, `dispatching-parallel-agents`, `executing-plans`, `finishing-a-development-branch`, `receiving-code-review`, `requesting-code-review`, `subagent-driven-development`, `systematic-debugging`, `test-driven-development`, `using-git-worktrees`, `using-superpowers`, `verification-before-completion`, `writing-plans`, `writing-skills` | Current Codex local environment or plugin cache; no standalone original link. | Structured AI coding workflows for planning, TDD, debugging, code review, worktrees, parallel agents, and completion verification. |
| Codex Context Ops | `context-agency-agents-install`, `context-bug-memory`, `context-feature-index`, `context-governance`, `context-init`, `context-release-check`, `context-safe-bugfix`, `context-safe-refactor`, `context-safe-review`, `context-subagents`, `context-worktree` | Current Codex local environment or plugin cache; no standalone original link. | Context management, feature indexing, agent installation, safe bugfix / refactor / review, worktrees, and release checks. |
| Sales | `analyze-account-signals`, `build-business-case`, `build-competitive-brief`, `enrich-company-and-contact-data`, `find-customer-quotes`, `find-key-internal-sources`, `follow-up-after-call`, `get-rep-call-feedback`, `hubspot`, `index`, `plan-deal-strategy`, `prepare-for-meeting`, `prioritize-accounts`, `review-forecast`, `review-rep-call-trends`, `sales-company-research`, `salesforce`, `suggest-sales-next-step`, `user-context`, `zoominfo` | Current Codex local environment or plugin cache; no standalone original link. | Sales workflows for meeting prep, call follow-up, account research, forecast review, competitive briefs, CRM, and contact enrichment. |

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

#### Detailed Description

`openai/skills` is the official skill catalog for Codex. A skill is a folder of instructions, scripts, and resources that an AI coding agent can load when a task matches a specific workflow. This repository is useful because it separates repeatable agent behavior from one-off prompts: instead of explaining the same workflow every time, you install the skill once and let Codex discover it when needed.

The catalog includes system skills that ship with Codex, curated skills for common workflows, and experimental skills for newer patterns. It is best treated as the canonical reference for learning how Codex skills are structured, what a `SKILL.md` should contain, and how official skills package supporting scripts or references.

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

#### Detailed Description

`forrest-orr/artifacts-kit` is not an AI-agent skill. It is a security research toolkit that can create pseudo-malicious user-mode memory artifacts on Windows so analysts can study, test, or demonstrate detection behavior. It focuses on memory allocation and execution patterns that resemble real malware footprints, which makes it useful for defensive research but unsuitable for normal Codex skill installation.

For this documentation, it is included as a related security resource rather than a Codex skill. The important note is separation: keep it out of `~/.codex/skills/`, do not present it as an agent instruction package, and only use it in controlled environments where this kind of artifact generation is authorized.

#### Install In Codex

This is not a Codex skill and should not be installed as one. Keep it as a separate security research reference.

#### How To Use

- Use only in an authorized lab or malware-analysis training environment.
- The repository is useful for understanding pseudo-malicious Windows memory artifacts and detection/testing scenarios.
- Do not mix it into normal Codex skill folders; document it separately because its purpose and risk profile are different from agent instruction skills.

### greensock/gsap-skills

#### Original Link

- Source: <https://github.com/greensock/gsap-skills>

#### Detailed Description

`greensock/gsap-skills` is the official Agent Skills package for GSAP, the GreenSock Animation Platform. It teaches AI coding agents the correct way to use GSAP APIs, including core tweens, timelines, ScrollTrigger, plugins, utility helpers, framework lifecycle cleanup, and performance-sensitive animation practices.

This is valuable because animation code often fails in subtle ways: missing plugin registration, unsafe React effects, selectors that leak outside component scope, scroll animations that need refresh handling, or layout properties that perform poorly. These skills give Codex a strong default playbook for generating maintainable GSAP animation in React, Vue, Svelte, and vanilla JavaScript projects.

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

#### Detailed Description

`pbakaus/impeccable` is a frontend design skill system that gives AI agents a richer vocabulary for visual quality. It is not just a single style guide: it includes a design skill, references for typography, color, spacing, motion, interaction, responsive design, and UX writing, plus command-style workflows such as audit, critique, polish, harden, animate, layout, and clarify.

The main purpose is to help AI avoid common generic UI patterns and make more deliberate product-design decisions. It is useful when a project needs higher visual taste, design-system alignment, responsive QA, accessibility checks, better copy, or a final polish pass before shipping.

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

#### Detailed Description

`Leonxlnx/taste-skill` is a collection of portable agent skills aimed at improving AI-generated frontend design. Its default skill focuses on stronger layout, typography, spacing, motion, and design-language inference so the UI does not look like a generic template. It also includes stricter GPT/Codex-oriented variants, redesign workflows for existing projects, image-to-code workflows, and style-specific options such as minimalist, high-end, or brutalist UI.

This repository is especially useful when the problem is not technical correctness but visual blandness. It helps Codex reason about design direction, choose stronger compositions, avoid placeholder-like output, and use reference images or brand boards as a bridge between visual exploration and implementation.

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

#### Detailed Description

`jnMetaCode/superpowers-zh` is a Chinese enhanced edition of the Superpowers skill framework. It turns AI coding from an ad-hoc "start writing code immediately" behavior into a disciplined workflow that includes brainstorming, planning, test-driven development, systematic debugging, code review, worktree isolation, and verification before completion.

Compared with the English upstream, this version adds Chinese translations, broader tool support, and China-specific workflow skills. It is useful for Chinese-speaking developers who want Codex to ask better questions, produce clearer plans, follow stricter engineering habits, and communicate in a style that fits domestic teams and Chinese technical documentation.

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

#### Detailed Description

`jnMetaCode/agency-agents-zh` is a Chinese community edition of the Agency Agents collection. Instead of describing one workflow, it provides a large library of specialist AI roles. Each role has an identity, domain expertise, process, and expected deliverables, so Codex can work as a frontend expert, product strategist, tester, marketer, legal reviewer, support specialist, or China-market operator depending on the task.

This edition translates upstream roles and adds China-specific agents for platforms and scenarios such as Xiaohongshu, Douyin, WeChat, Bilibili, Feishu, DingTalk, cross-border ecommerce, government/enterprise workflows, and compliance-heavy industries. It is best used when a task needs a clear expert perspective rather than a generic assistant voice.

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

#### Detailed Description

`msitarzewski/agency-agents` is the English upstream collection of specialist AI agents. It is organized like an agency: each agent has a specific professional identity, communication style, workflows, deliverables, and success metrics. The collection spans engineering, design, product, marketing, sales, finance, security, testing, strategy, support, and other domains.

The value of this repository is role precision. Instead of asking Codex to "act like an expert" from scratch, you can install or reference a prepared agent definition that tells the model how that expert thinks, what process to follow, and what output quality looks like.

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
