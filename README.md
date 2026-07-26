# Practice to Principles

[English](#english) · [中文](#中文)

## English

`practice-to-principles` turns meaningful applications of external knowledge into scoped, evidence-backed, reusable principles.

It is designed to work alongside book-derived and other knowledge skills. Source material remains source material; only lessons supported by real decisions, actions, or reviews enter the learning pipeline.

### How it works

```text
Knowledge skill
      ↓ applied to real work
Application episode
      ↓ evidence and reflection
Candidate principle
      ↓ repeated support + user confirmation
Activation plan
      ↓ authorized route + load verification
Active principle
```

The skill:

- ignores simple lookups, summaries, and episodes without meaningful evidence;
- records source, scope, triggers, exceptions, support, and counterevidence;
- merges overlapping observations instead of accumulating duplicates;
- requires repeated practical support, explicit user confirmation, and a verified activation route before promotion;
- preserves rejected or superseded principles instead of silently deleting history;
- never rewrites system instructions, project rules, or external memory without target-specific authorization.

### Structure

```text
practice-to-principles/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── active.md
    ├── candidates.md
    └── retired.md
```

The core prompt stays intentionally small. `active.md` is the canonical registry, not a global context source. A confirmed principle becomes active only after a concise execution hook is installed in a workflow that naturally loads it before the relevant action. Confirmed principles without a route remain `confirmed-unrouted` candidates.

The reference files may accumulate personal context. Review their contents before publishing later updates.

### Install

```powershell
git clone https://github.com/Anle-He/practice-to-principles.git "$HOME\.codex\skills\practice-to-principles"
```

Start a new Codex task after installation so the skill can be discovered.

### Use

Invoke it explicitly:

```text
$practice-to-principles distill what we learned from this application.
```

It can also be invoked implicitly after a knowledge framework materially affects a decision, action, or review and outcome evidence becomes available.

## 中文

`practice-to-principles` 将外部知识在真实任务中的有效应用，提炼为有范围、有证据、可复用的原则。

它适合与书籍型及其他知识型 skill 配合使用。来源中的观点仍然只是来源观点；只有经过真实决策、行动或复盘检验的认识，才会进入学习流程。

### 工作方式

```text
知识型 skill
    ↓ 用于真实任务
一次应用事件
    ↓ 结果证据与复盘
候选原则
    ↓ 重复支持 + 用户确认
激活计划
    ↓ 授权路由 + 加载验证
生效原则
```

这个 skill 会：

- 忽略单纯查询、内容概括以及缺少有效证据的应用；
- 记录来源、适用范围、触发条件、例外、支持证据与反证；
- 合并重复认识，避免原则无限堆积；
- 仅在多次实践支持、用户明确确认且激活路由验证通过后晋升原则；
- 保留被否定或替代的原则，不静默抹除历史；
- 未经目标级明确授权，不改写系统指令、项目规则或外部记忆。

### 文件结构

```text
practice-to-principles/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── active.md
    ├── candidates.md
    └── retired.md
```

核心 prompt 有意保持精简。`active.md` 是原则的唯一事实来源，并不是全局上下文。确认后的原则只有在相关工作流中安装精简执行钩子、且验证该工作流会在行动前自然加载它之后，才算 active；没有路由的确认原则继续保留为 `confirmed-unrouted` 候选。

引用文件可能逐渐包含个人情境；以后发布更新前，应先检查其中的内容。

### 安装

```powershell
git clone https://github.com/Anle-He/practice-to-principles.git "$HOME\.codex\skills\practice-to-principles"
```

安装后新建一个 Codex 任务，使 skill 被重新发现。

### 使用

可以显式调用：

```text
$practice-to-principles 提炼这次应用中值得长期保留的原则。
```

当某个知识框架实质性影响了决策、行动或复盘，并且已经出现结果证据时，也可以隐式触发。
