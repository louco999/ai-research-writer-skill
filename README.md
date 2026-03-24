# ai-research-writer.skill

一个面向长流程科研写作的 Agent Skill，强调过程可控、迭代打磨和稳定输出质量。

## 项目简介

`ai-research-writer.skill` 适用于需要多轮推理与持续改写的科研写作任务，核心思路包括：

- 长流程执行（long-running workflow），而不是一次性生成
- 分阶段写作与检查点控制，便于追踪质量
- 通过迭代修订提升论证清晰度、证据一致性与文本稳定性

该 skill 的设计灵感来自 Anthropic 的两篇研究：

- [Long-running Claude](https://www.anthropic.com/research/long-running-Claude)
- [Vibe Physics](https://www.anthropic.com/research/vibe-physics)

## 适用场景

你可以在以下任务中使用这个 skill：

- 把零散笔记整理为结构完整的研究初稿
- 按“提纲 -> 分节撰写 -> 交叉校对 -> 终稿润色”的流程工作
- 在长文写作中保持术语、结构和语气的一致性
- 通过流程约束与复核回路降低幻觉和逻辑跳步

## 推荐工作流

1. 明确写作目标、受众、约束条件与交付格式。
2. 先产出可审阅的结构化提纲。
3. 按章节扩写，优先证据与论点对齐。
4. 进行多轮修订（逻辑、事实、表达、风格）。
5. 输出终稿，并按需生成摘要版/演示版。

## 仓库内容

- `ai-research-writer.skill`：技能文件本体
- `README.md`：项目说明与使用建议

## 后续可扩展项

- 增加输入/输出样例（example cases）
- 增加写作质量评估清单（rubric）
- 增加固定 benchmark 任务用于复现实验

