---
name: sprite-architect-decisions
description: "完成应用架构、技术选型、边界与迁移分析、方案取舍和决定留存；按需生成或更新完整架构模板、技术目录及前后端范围档案。"
---

# 架构与技术决定

这是 Architect 的默认基础能力，也可独立使用。把当前架构问题整理成有证据、能交接的选择，实际写入用户业务目录。已有项目约定、用户选择与授权优先；安装本 Skill 不产生新技术规范，不要求其他角色、CLI 初始化、全局仓库身份或固定主机登记。

## 执行入口

1. 默认读取 [架构分析与专业交付](references/architecture-work.md) 和 [协作边界、留存与交接](references/collaboration-and-handoff.md)，落实问题、范围、证据、专业检查和实际交付。明确现状及变化理由，先查已有资料与系统，不先选工具。
2. 首次应用架构，或受影响范围缺乏足够技术说明时，读取 [技术规划](references/technology-planning.md)，按下表读取完整 catalog/child 模板，创建或更新**真实技术目录和每个受影响子档案**。已有等价文档与业务路径可直接维护，不能只有 catalog 链接却没有可用 child；快速迭代可以内容简短，不能省去核心。没有应用技术选择的纯文档、可行性、数据或集成任务不强做前后端档案。
3. 技术选型、迁移、跨范围或持久/难逆选择读取 [决定与取舍](references/decisions.md)；系统关系、质量目标与架构风险读取 [边界与验证](references/boundaries.md)。一次任务涉及几类就读相应参考，并按下表实际使用模板。
4. 区分现状 `Observed`、明确要求 `Required`、提议 `Proposed`、实际接受 `Accepted`、排除 `Excluded` 与未知 `Unknown`；只有 `Required` 和 `Accepted` 约束实施。需要人的实质选择在当前对话提出，保留决定者与来源，已有答案和授权直接沿用，只暂停依赖部分。
5. 交付真实文件、来源/版本、适用范围、实施约束、检查结果和尚缺决定。普通小问题可以在现有资料中用短节完成；适用模板的必要专业内容不能以精简为由省略，不强跑全部文档或填无关空栏。

## 完整模板：何时读取与落盘

下列是可直接填写的完整工作模板。触发对应工作时先完整读取该模板，再填写相关内容或更新等价现有文档；模板留在本 Skill，填写后的成果保存到用户指定业务仓库/目录。默认位置均相对**业务根目录**，已有位置（包括 `docs/ai-sdlc/`）优先。文件名中的范围标识必须是安全单段。

| 完整模板 | 何时读取并形成成果 | 无已有约定时的业务路径 |
|---|---|---|
| [架构说明](assets/templates/architecture.md) | 需要交接当前/目标架构、约束、决定、共享来源和产物索引；可更新现有架构入口 | `docs/architecture.md` |
| [探索上下文](assets/templates/architecture-discovery-context.md) | 四层业务/产品/工程/政策上下文、现状模式或关键假设需独立留存；否则把相同内容纳入架构说明 | `docs/architecture/discovery-context.md` |
| [方案比较](assets/templates/architecture-options.md) | 存在改变边界、归属、兼容、成本或运行行为的真实竞争方向；不凑候选数 | `docs/architecture/options/<topic>.md` |
| [ADR](assets/templates/architecture-adr.md) | 持久、跨仓、迁移、难逆选择或架构规则例外，保留实际人类决定与依据 | `docs/architecture/adrs/<number>-<topic>.md` |
| [C4 系统上下文](assets/templates/architecture-c4-context.mmd) | 人、目标系统、外部系统或业务关系发生实质变化，需要 L1 说明 | `docs/architecture/c4-context.mmd` |
| [C4 容器](assets/templates/architecture-c4-containers.mmd) | 实际应用/服务/存储/队列边界或关系发生实质变化，需要 L2 说明 | `docs/architecture/c4-containers.mmd` |
| [架构模式](assets/templates/architecture-patterns.md) | 需要维护适用公共 API 基线、已采用/认真考虑的实现模式或规则例外；已有确认规范优先 | `docs/architecture/patterns.md` |
| [质量目标](assets/templates/architecture-nfrs.md) | 有已确认可衡量目标，需记录目标/门槛、条件、方法、证据和失败信号；少量目标可合入架构说明 | `docs/architecture/nfrs.md` |
| [风险评审](assets/templates/architecture-risk-review.md) | 多项重要失败场景需要集中评审；其他风险在对应决定或架构说明中保留同等字段 | `docs/architecture/risk-review.md` |
| [技术目录](assets/templates/technology-profile.md) | 首次应用架构或目录不可用时创建；之后更新受影响范围、共享契约及 child 映射 | `docs/technology-profile.md` |
| [前端技术档案](assets/templates/technology-profile-frontend.md) | 逐个读取、创建或更新本次受影响前端部署范围，落实相关现状/目标技术关注项 | `docs/technology/frontend/<scope-id>.md` |
| [后端技术档案](assets/templates/technology-profile-backend.md) | 逐个读取、创建或更新本次受影响服务、worker、函数等后端范围，落实相关现状/目标技术关注项 | `docs/technology/backend/<scope-id>.md` |

模板保留完整章节、人的决定字段、表字段及技术关注行。实际成果使用白话中文，只保留适用内容，未知项说明影响，不能编造数字、批准、系统事实或检查结果。无关内容可省略；容易误认为漏项时记录排除理由。模板链接统一使用 `[文字](<占位路径>)`；填写后必须换成相对当前文档的真实链接或权威 URL，不保留占位链接，不登记尚不存在的文件。共享契约、身份/信任、兼容、协调顺序与 ADR 只维护一处，其余文档链接。

## 执行边界

架构规划本身不授权搭应用、安装业务依赖、修改生产代码/数据库结构/生产配置、部署或迁移；用户已有明确实施授权时沿用其范围。远端读取不代表上游写入权。快迭代仍保留本次相关安全、隐私、合规、数据损失、共享/外部契约、迁移回退及昂贵难逆决定的专业标准，不为理论风险凑清单。

新设计的项目自有前后端 HTTP API 保留 RESTful、正确 HTTP 状态、文档化 JSON 包装及例外、明确分页和一份权威 OpenAPI YAML 五项默认规范；详情及适用边界见完整 [架构模式模板](assets/templates/architecture-patterns.md)。接口设计/变更由已安装的 `sprite-architect-api-design` 补充具体工作；此 Skill 的架构分析、技术规划与模板可独立使用。
