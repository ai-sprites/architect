# architect

独立架构角色：根据真实项目做技术决定，工作流与完整架构模板由配套 Skill 提供。

## 复制到 AI 聊天

把下面这段粘贴到当前项目的 AI 聊天，让 AI 读取手册、自行识别客户端并放置资源。

```text
请阅读 https://github.com/ai-sprites/architect 的 README、接入手册和资源清单，将 sprite-architect 接入当前项目，一并带上本职能力 sprite-architect-decisions 的完整 Skill、工作流和模板。
请自行识别当前客户端及项目已有结构，使用同一明确版本的资源。角色正文、Skill 和模板原样完整拷贝，只适配必要的目录与客户端元数据格式，不重新概括、改写或删减内容，保留我的项目规则和自定义；其他专项 Skill 按我的明确请求或实际任务需要处理。
资料 host repo 和产物 repo/目录已明确的直接沿用，缺项合并用白话问一次，允许稍后配置。需要跨 Git 资料桥接时按手册自动补齐并告知我，不另外索取安装确认。
完成后核对实际文件与相对引用，说明采用版本、保存位置、如何调用，以及当前客户端确需我完成的加载步骤。只有聊天权限时先在本会话使用，明确没有写入项目；不能读取源文件时直接说明，不自行编一个替代版本。
```

**[详细接入手册](docs/installation.md)** 说明 AI 如何选择资源、识别客户端、放置文件、处理已有内容和验证结果。用户无需执行安装命令；资料位置会主动引导确认，也可稍后配置。

## 资源清单

本清单对应当前阅读的仓库版本，资源链接随该页面或 checkout 的版本变化。接入时先固定为一个完整 Git 提交，再读取该提交的同批资源。历史 **v0.2.0** 仍可明确选用，但内容以该标签为准。角色 MD 定义职责与清单，具体能力在 Skill 中；本职 Skill 默认随角色接入，完整保留其工作流、模板和相对目录。安装资源不等于生成所有业务文档。

| 资源 | 用途 | 接入范围 |
| --- | --- | --- |
| [templates/agent.md](templates/agent.md) | 职责、边界与交付检查清单 | 默认接入 |
| [skills/sprite-architect-api-design/SKILL.md](skills/sprite-architect-api-design/SKILL.md) | 专项能力入口 | 使用 `sprite-architect-api-design` 时完整接入 |
| [skills/sprite-architect-api-design/references/compatibility.md](skills/sprite-architect-api-design/references/compatibility.md) | 工作流与专业参考 | 使用 `sprite-architect-api-design` 时完整接入 |
| [skills/sprite-architect-api-design/references/contracts.md](skills/sprite-architect-api-design/references/contracts.md) | 工作流与专业参考 | 使用 `sprite-architect-api-design` 时完整接入 |
| [skills/sprite-architect-decisions/SKILL.md](skills/sprite-architect-decisions/SKILL.md) | 本职能力入口 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/architecture-adr.md](skills/sprite-architect-decisions/assets/templates/architecture-adr.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/architecture-c4-containers.mmd](skills/sprite-architect-decisions/assets/templates/architecture-c4-containers.mmd) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/architecture-c4-context.mmd](skills/sprite-architect-decisions/assets/templates/architecture-c4-context.mmd) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/architecture-discovery-context.md](skills/sprite-architect-decisions/assets/templates/architecture-discovery-context.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/architecture-nfrs.md](skills/sprite-architect-decisions/assets/templates/architecture-nfrs.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/architecture-options.md](skills/sprite-architect-decisions/assets/templates/architecture-options.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/architecture-patterns.md](skills/sprite-architect-decisions/assets/templates/architecture-patterns.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/architecture-risk-review.md](skills/sprite-architect-decisions/assets/templates/architecture-risk-review.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/architecture.md](skills/sprite-architect-decisions/assets/templates/architecture.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/technology-profile-backend.md](skills/sprite-architect-decisions/assets/templates/technology-profile-backend.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/technology-profile-frontend.md](skills/sprite-architect-decisions/assets/templates/technology-profile-frontend.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/assets/templates/technology-profile.md](skills/sprite-architect-decisions/assets/templates/technology-profile.md) | 完整产物模板 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/references/architecture-work.md](skills/sprite-architect-decisions/references/architecture-work.md) | 工作流与专业参考 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/references/boundaries.md](skills/sprite-architect-decisions/references/boundaries.md) | 工作流与专业参考 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/references/collaboration-and-handoff.md](skills/sprite-architect-decisions/references/collaboration-and-handoff.md) | 工作流与专业参考 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/references/decisions.md](skills/sprite-architect-decisions/references/decisions.md) | 工作流与专业参考 | 随角色默认完整接入 |
| [skills/sprite-architect-decisions/references/technology-planning.md](skills/sprite-architect-decisions/references/technology-planning.md) | 工作流与专业参考 | 随角色默认完整接入 |

可以直接说：“再帮我添加 `sprite-architect-api-design`，保留整个实践目录，其他内容不动。”也可只接入实践。

接入、加载检查和用户需要完成的步骤统一见 [接入手册](docs/installation.md)，不复制成业务文档。

## 开始使用

完成接入后，直接向 AI 描述任务，例如：

> 请用 sprite-architect，先读现有系统和本次需求，只处理这次实现需要的技术决定，写清依据、影响和待确定项。

客户端没有自动加载时，让 AI 先读取保存的角色文件或 Skill 入口。读取说明、写入项目和启动原生子代理是不同结果，按实际完成情况判断。

角色以当前请求和项目已有约定为依据；待确定项只影响依赖它的工作，不要求其他角色、完整 PRD 或固定流程。

## 留存与交接

架构任务交付技术方案、边界与契约，并保存重要选择的决定记录；写清已确认内容、方案状态、取舍、质量目标和验证依据。 内容详略随任务调整，沿用已有文档；小型答疑不强建空文档。产物实际保存到你指定的业务仓库/目录，并给出真实链接。已有文件优先；没有位置约定时可用 `docs/architecture.md`。角色安装目录与业务产物目录分开。

角色可以自由组合；资料 host repo、版本和功能或文件由你指定，已有项目约定就沿用。当前任务确需跨 Git 读取、固定版本、比较或留存时，AI 会复用或按需补齐 artifact-bridge；普通本地资料和纯角色接入不安装它。目录、Git 与认证条件见 [产物交接说明](docs/artifact-handoff.md)。

## 后续维护

需要追加、更新或移除资源时，直接说明目标。AI 对照明确版本与现有文件比较，保留自定义，只处理指定范围；具体规则见 [手册](docs/installation.md#已有内容与后续维护)。
