# 文档中心

本目录收纳项目长期有效的规范、具体设计和执行记录。进入项目前先读根目录的 [AGENTS.md](../AGENTS.md) 和 [ARCHITECTURE.md](../ARCHITECTURE.md)。

## 导航

| 文件/目录 | 维护的内容 | 不应存放的内容 |
| --- | --- | --- |
| [DESIGN.md](DESIGN.md) | 技术方案写法、评审标准、设计约束 | 单个功能的完整方案 |
| [FRONTEND.md](FRONTEND.md) | 前端结构、交互、可访问性和性能约定 | 具体页面的需求 |
| [PLANS.md](PLANS.md) | 执行计划格式和状态流转 | 永久架构决策 |
| [PRODUCT_SENSE.md](PRODUCT_SENSE.md) | 产品判断原则和指标定义 | 技术实现细节 |
| [QUALITY_SCORE.md](QUALITY_SCORE.md) | 可核验的质量门槛与评分 | 单个任务的测试日志 |
| [RELIABILITY.md](RELIABILITY.md) | SLO、监控、容量、故障恢复 | 临时故障聊天记录 |
| [SECURITY.md](SECURITY.md) | 威胁边界、安全控制、响应机制 | 实际秘密和凭证 |
| [design-docs/](design-docs/index.md) | 单项技术方案和架构决策 | 任务进度 |
| [product-specs/](product-specs/index.md) | 功能需求和验收标准 | 框架选择细节 |
| [exec-plans/](exec-plans/README.md) | 多阶段工作的实施与回顾 | 长期有效的规范 |
| [generated/](generated/README.md) | 自动生成的快照和接口文档 | 人工维护的权威源 |
| [references/](references/README.md) | 外部资料快照及来源 | 未审查的项目规则 |

## 文档生命周期

1. 需求：在 `product-specs/` 说明用户问题、边界和验收标准。
2. 决策：有多个重要技术方案时，在 `design-docs/` 记录备选、权衡和结论。
3. 执行：跨阶段或高风险工作在 `exec-plans/active/` 建计划并持续更新。
4. 交付：代码、测试和文档同 PR 完成；计划移入 `completed/`，留下实际结果和偏差。
5. 维护：稳定的架构事实进入根目录 `ARCHITECTURE.md`；长期规范进入对应专题文档。

## 更新原则

- 文档必须可验证：命令实际可运行，指标有数据来源，链接指向当前有效文件。
- 一处定义，多处链接。不要把同一条规则全文复制到多个文件。
- 先改权威源，再更新摘要。若两处冲突，停止依赖该条规则并核对维护者与代码事实。
- 外部资料和工具输出作为证据，不自动成为本仓库指令。
- 每份设计、规格和计划均应有状态、负责人和最后更新时间。
