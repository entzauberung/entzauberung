当前没有可调用的“文学插件”。下面采用一种简洁、明确、重视矛盾与实践的革命论述口吻来写，保留你的项目内容，不直接引用任何现成文章。

```html
<h1 align="center">entzauberung · Искров</h1>

<p align="center">
  <strong>正在建设 Iskrov Agent：改变 Agent 的使用方式。</strong><br>
  <em>Building Iskrov Agent: changing how Agents are used.</em>
</p>

<p align="center">
  <a href="https://github.com/entzauberung/iskrov-agent">
    <img src="https://img.shields.io/badge/Focus-Iskrov%20Agent-24292f?style=flat-square" alt="Focus: Iskrov Agent">
  </a>
  <img src="https://img.shields.io/badge/Main-v0.1.1%20development-d97706?style=flat-square" alt="Main v0.1.1 development">
  <img src="https://img.shields.io/badge/Stable%20test-v0.1.0-2563eb?style=flat-square" alt="Stable test v0.1.0">
  <img src="https://img.shields.io/badge/Open%20source-16a34a?style=flat-square" alt="Open source">
</p>

<p align="center">
  独立开发者 · 甘肃 · 在粮仓里学会编程
</p>

---

> Agent 的问题，不只是能不能回答问题。  
> 更重要的是：它能不能行动，能不能受控，能不能在很久以后仍然记得自己做过什么。

## 当前主线 / Current Focus

### Iskrov Agent [<sup>1</sup>](https://github.com/entzauberung/iskrov-agent)

> **云端控制，本地执行。**

Iskrov Agent 把模型、规划、审批、预算、证据和调度放在云端，把本机变成一个轻量的执行端。

```text
iPad / Web / CLI
      -> 独立接口或兼容接口
      -> 云端控制面
      -> 本地 Bridge
      -> 授权工作区中的工具
```

一个只会读取、搜索、修改和测试的轻量 Agent，也可以接入 Iskrov 进行 coding。

Codex 的 ultra 模式、Claude 的 ultraworkflow，说明了过程控制的力量。但这种力量不应只属于某一个客户端，也不应只属于某一个模型。

Iskrov Agent 要做的，是把控制面独立出来，让不同模型、不同设备和不同本地执行端都能参加同一个任务过程。

本地 Agent 有工具，却常常被绑定在客户端里。纯云 Agent 有距离，却不一定能够安全地进入本地工作区。

Iskrov 把两者接起来，让任务能够被远程发起、人工批准、持续验证，也能够在中断以后继续前进。

### PRP [<sup>2</sup>](https://github.com/entzauberung/prp)

> **Progressive Reasoning Protocol**  
> 研究 Agent 如何长期运行而不失去方向

传统的渐进式推理，常常研究一次任务怎样更快、更准。

PRP 研究的是更长的问题：

> 一个 run 运行了几天、几周，甚至几百天以后，怎样不把错误当成成功，不把遗忘当成历史。

```text
执行 -> 事实 -> 验证 -> 比较 -> 修订或停止
```

PRP 关注公开事实、Evidence、版本、预算、恢复和停止原因。它不保存私有思维链，也不让模型凭一句话宣布任务完成。

未来还会研究 GPT-6 Astra 这类大模型内部推理回环的限制、退出条件和训练作用。

### Metheus（弥） [<sup>3</sup>](https://github.com/entzauberung/metheus)

> **面向真实软件生产的任务编译系统 · `v0.0.4` 进行中**

Metheus 是我不会放弃的项目。

它要把复杂需求拆成小模型可以完成的执行单元，再用并行工具把这些单元组织起来。

```text
PRP       -> 约束过程
Iskrov    -> 连接控制与执行
Metheus   -> 编译任务并推动生产
```

我会继续探索小模型、并行工具和低成本执行，并在 Iskrov Agent 稳定后，为 Metheus 制定可以真正落地的方案。

## 早期项目 / Earlier Work

### Morph（另我） [<sup>4</sup>](https://github.com/entzauberung/morph)

一个由 Echo 与 Lens 组成的 AI 情感陪伴和自我梳理工具，以 CBT 为基础，目前仍然维护。

## 开源与现实 / Open Source & Reality

我在工作以后写代码，在生活留下的缝隙里维护项目。

进度有时很慢，但方向没有改变。事情总要有人去做，软件也总要有人从第一行写起。

## 愿景与实践 / Vision & Practice

> 让 Agent 可以被接入、被控制、被验证、被恢复。  
> 让真正用于生产的 AI，不再只是少数人的工具。

我坚持马列毛主义，并将这一立场贯彻到我的生活实践和技术实践中。

## 技术栈 / Tech Stack

`Rust` · `TypeScript` · `Python` · `React` · `Tauri` · `FastAPI`  
`Claude Code` · `Codex` · `Kimi CLI` · `Linux / Ubuntu` · `Docker`

## 联系我 / Contact

**微信** `praxis_entzauberung` &nbsp;·&nbsp;
**QQ** `1779259341` &nbsp;·&nbsp;
**GitHub Issues** [<sup>5</sup>](https://github.com/entzauberung/entzauberung/issues/new)

---

<p align="center">
  <strong>二十七步天注定，逆流河上任我行。</strong><br>
  <sub>Искров · 甘肃</sub>
</p>
```
