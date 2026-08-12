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

> **当前主产品 · `v0.0.4` 进行中**

Metheus 是这条全小模型路线的主要实践载体。小模型不是降级方案，而是目标执行形态。

| 版本 | 状态 | 方向 |
| :--- | :---: | :--- |
| `v0.0.4` | **进行中** | 第二阶段：hermes记忆模式，轻度机器学习，但是分级做到成本控制<br>第三阶段：实现由决策层向执行单元分派任务 |
| `v0.0.5` | 计划 | 全面定制 Grok Build，将执行层推进为并行执行 |
| `v0.0.6` | 计划 | 接入 PRP 的 Metheus 特化实现 |

### PRP [<sup>3</sup>](https://github.com/entzauberung/prp)

> **通用协议 · 厂商无关 · 可独立部署**

PRP（Progressive Reasoning Protocol）是通用的渐进式推理与执行编排协议。

它希望把原本封装在 Codex、Claude Code 等 Agent 客户端内部的渐进式工作流，抽象成可以独立部署、跨客户端和模型后端复用的通用协议层。

**接口：** `PRP Native` · `OpenAI Responses` · `OpenAI Chat Completions` · `Anthropic Messages`

在目标形态中，用户只需在终端或兼容客户端中配置 PRP 服务端点，就能接入不同模型后端，获得同类的渐进式组织与执行能力。

### metheus-prp [<sup>4</sup>](https://github.com/entzauberung/metheus-prp)

> **面向 Metheus `v0.0.6` 的全小模型特化实现**

它不采用“强模型决策、弱模型执行”的分层路线，而是让所有执行单元完全由小模型处理，面向高并发、高吞吐和更低的单位 token 成本进行极致优化。

## 早期项目 / Earlier Work

### Morph（另我） [<sup>5</sup>](https://github.com/entzauberung/morph)

由 Echo（艾可）与 Lens（棱镜）组成的CBT认知行为疗法为内核的 AI 情感陪伴与自我梳理工具。它是我较早完成的项目，目前仍在维护，但已经不是现在的主要重心。

## 开源与现实 / Open Source & Reality

我已经把自己的生活、时间和精力全部投入开源事业，目前主要围绕 Metheus 与 PRP 推进。

这两个项目没有团队和充足资金，也不是在理想条件下开发的。目前，我把包括饭钱在内的全部生活费投入 API token，这让日常生活和项目更新都异常艰难，但开发仍在继续。

## 愿景与实践 / Vision & Practice

> 我的五年目标，是通过持续的系统性优化，把 AI 执行的 token 成本压到接近电费的量级，让每个人都能以一杯奶茶的价格，使用更快、更便宜、真正可以用于生产的 AI。

我坚持马列毛主义，并将这一立场贯彻到我的生活实践和技术实践中。

## 技术栈 / Tech Stack

**语言** `Rust` · `TypeScript` · `Python` &nbsp;|&nbsp; **框架** `React` · `Tauri` &nbsp;|&nbsp; **工具与环境** `Claude Code` · `Codex` · `Kimi CLI` · `Grok Build` · `Linux / Ubuntu` · `Docker`

## 联系我 / Contact

**微信** `praxis_entzauberung` &nbsp;·&nbsp; **QQ** `1779259341` &nbsp;·&nbsp; **GitHub Issues** [<sup>6</sup>](https://github.com/entzauberung/entzauberung/issues/new)

---

<p align="center">
  <strong>二十步天注定，逆流河上任我行。</strong><br>
  <sub>Искров · 甘肃</sub>
</p>
