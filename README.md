<h1 align="center">entzauberung · Искров</h1>

<p align="center">
  <strong>正在构建 Metheus（弥）：面向真实软件生产的 AI 任务编译系统。</strong><br>
  <em>Building Metheus, an AI task compiler for real software production.</em>
</p>

<p align="center">
  <a href="https://github.com/entzauberung/metheus">
    <img src="https://img.shields.io/badge/Focus-Metheus-24292f?style=flat-square" alt="Focus: Metheus">
  </a>
  <img src="https://img.shields.io/badge/Status-v0.0.4%20in%20progress-d97706?style=flat-square" alt="v0.0.4 in progress">
  <img src="https://img.shields.io/badge/Direction-small--model%20execution-2563eb?style=flat-square" alt="Small-model execution">
  <img src="https://img.shields.io/badge/Work-open%20source-16a34a?style=flat-square" alt="Open source">
</p>

<p align="center">
  高二因双相情感障碍和语言障碍休学 · 甘肃农村 · 在粮仓里自学编程
</p>

---

> **我正在探索一条全小模型路线：**  
> 将原本需要大模型整体处理的复杂需求，编译成小模型可以独立完成的执行单元，以高并发、高吞吐的并行执行降低 token 成本。

## 当前主线 / Current Focus

### Metheus（弥） [<sup>2</sup>](https://github.com/entzauberung/metheus)

> **当前主产品 · `v0.0.4` 进行中，但是落地时间很长，后续重构grokbuild我估计要面临生存危机，目前重心在PRP协议上**

Metheus 是这条全小模型路线的主要实践载体。小模型不是降级方案，而是目标执行形态。

| 版本 | 状态 | 方向 |
| :--- | :---: | :--- |
| `v0.0.4` | **进行中** | 第二阶段：hermes记忆模式，轻度机器学习，但是分级做到成本控制<br>第三阶段：实现由决策层向执行单元分派任务 |
| `v0.0.5` | 计划 | 全面定制 Grok Build，将执行层推进为并行执行 |
| `v0.0.6` | 计划 | 接入 PRP 的 Metheus 特化实现 |

### PRP [<sup>3</sup>](https://github.com/entzauberung/prp)

> **通用协议 · 厂商无关 · 面向真实软件生产的任务编译与渐进式执行协议**

PRP（Progressive Reasoning Protocol）不是让单个模型一次性解决复杂需求的提示词模板，也不是某一家模型服务的封装层。

它试图把复杂的软件任务编译成一组可执行、可验证、可恢复、可审批、可停止的执行单元，并在执行过程中持续记录任务状态、上下文、工具调用、权限、证据、变更和失败原因。

PRP不规定必须使用大模型还是小模型。它提供的是一套独立于模型能力的组织方式：让模型负责判断和执行，让协议负责约束过程，让工具、权限、Workspace、Evidence和恢复机制共同构成一条可追踪的生产链。

它希望把原本封装在 Codex、Claude Code 等 Agent 客户端内部的渐进式工作流，抽象成可以独立部署、跨客户端和模型后端复用的协议层。未来，复杂任务可以在进入执行阶段前被进一步拆解为适合不同模型、不同权限和不同成本约束的执行单元。

**接口：** `PRP Native` · `OpenAI Responses` · `OpenAI Chat Completions` · `Anthropic Messages`

在目标形态中，用户只需在终端或兼容客户端中配置 PRP 服务端点，就能接入不同模型后端，获得统一的任务编排、执行追踪、审批控制、证据记录和失败恢复能力。

PRP是Metheus全小模型路线所依赖的通用协议基础；而Metheus则进一步探索，如何把复杂任务编译成小模型能够独立完成、并且可以高并发并行执行的具体单元。

### metheus-prp [<sup>4</sup>](https://github.com/entzauberung/metheus-prp)

> **面向 Metheus `v0.0.6` 的全小模型特化实现**

它不采用“强模型决策、弱模型执行”的分层路线，而是让所有执行单元完全由小模型处理，面向高并发、高吞吐和更低的单位 token 成本进行极致优化。

## 早期项目 / Earlier Work

### Morph（另我） [<sup>5</sup>](https://github.com/entzauberung/morph)

由 Echo（艾可）与 Lens（棱镜）组成的CBT认知行为疗法为内核的 AI 情感陪伴与自我梳理工具。它是我较早完成的项目，目前仍在维护，但已经不是现在的主要重心。

## 开源与现实 / Open Source & Reality

我曾经希望把全部的生活、时间和精力投入开源事业，但现实并没有给我这样的条件。

为了糊口，我不得不去电子厂拧螺丝，用流水线上的劳动换取一份勉强维持生活的收入。白天的时间和体力被工作切走，等到下班回到代码面前，很多时候已经只剩下疲惫，以及第二天还要继续工作的现实。

所以现在的开发，并不是在理想条件下持续推进，也不是一种从容而高效的个人选择。项目的计划会被工作打断，更新会变慢，原本可以连续完成的事情只能被拆成零碎的夜晚和休息日。有些时候，不是没有想法，也不是不愿意继续，而是身体、时间和生活已经没有更多可以交出来的东西。

这不是一个励志故事，也不是我愿意接受的工作方式。它只是当前生活条件下，为了继续活下去而不得不做出的安排。

我仍然在尽力维护 Metheus、PRP 和其他项目。只是现在，我只能在被流水线切碎的时间里，尽量保住开发的连续性，把还能留下来的精力投入代码、设计和实验之中。

开源对我来说不再只是兴趣或职业规划，而是在非常有限的条件下，仍然试图保留下来的一条道路。它走得很慢，也经常被现实推回原点，但目前还没有停止。

## 愿景与实践 / Vision & Practice

> 我的五年目标，是通过持续的系统性优化，把 AI 执行的 token 成本压到接近电费自来水费的量级，让每个人都能以一杯奶茶的价格，使用更快、更便宜、真正可以用于生产的 AI。

我坚持马列毛主义，并将这一立场贯彻到我的生活实践和技术实践中。

## 技术栈 / Tech Stack

**语言** `Rust` · `TypeScript` · `Python` &nbsp;|&nbsp; **框架** `React` · `Tauri` &nbsp;|&nbsp; **工具与环境** `Claude Code` · `Codex` · `Kimi CLI` · `Grok Build` · `Linux / Ubuntu` · `Docker`

## 联系我 / Contact

**微信** `praxis_entzauberung` &nbsp;·&nbsp; **QQ** `1779259341` &nbsp;·&nbsp; **GitHub Issues** [<sup>6</sup>](https://github.com/entzauberung/entzauberung/issues/new)

---

<p align="center">
  <strong>二十七步天注定，逆流河上任我行。</strong><br>
  <sub>Искров · 甘肃</sub>
</p>
