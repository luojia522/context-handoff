# context-handoff · 上下文交接（重启人机结合系统）

> 让人与 AI 的协作者关系，活过上下文压缩、换窗与冷启动。
> Let human–AI collaboration survive context compression, window switches, and cold starts.

[English summary below](#english-summary)

## 这是什么

一个 Kimi 插件（skill-only），把我们在长期人机协作中实证出的一套**上下文交接规程**固化为 AI 可自动加载的技能：

- **交（断线／压缩前自报）· 最小完备五栏**：当前口令／勿重做清单／勿 reopen 边界／工具链要点／缺口与风险——写给零上下文的接手者：路径写绝对、版本钉号码、动作带命令。
- **接（新会话载入）· 四步验收**：读接续笔记与工作单 → 按装机清单逐项核对在位 → 自报四点后停住等口令 → **回读验收对物证不对自述**（git log、落盘文件、登记簿交叉验证）。
- **装机清单核对 · 失败报告式**：缺失不硬撑，按「路径／预期／现状」三栏报人。
- **压缩观测立档**：每次上下文压缩皆立 00N 号档案；主动节奏＝主题收口即盘点，赶在系统强制压缩之前。
- **铁律**：判断与裁决永留人侧，任何适配层不得代裁。

## 为什么（实证来源）

2026-08-28，一次真实会话经历系统强制上下文压缩：凭预先落盘的「接续现场笔记」，新上下文**零障碍接续**了四件落实包任务——观测档案 001 号在案。生态佐证：DSH 1024Store 中 memory 类插件居安装榜头部，「agent 记不住」是整个 agent 生态的刚需。

方法论谱系：钱学森「人·机结合，以人为主」综合集成思想在 AI 协作工程中的落地——机器供给证据与计算，人执掌判别与裁定。

## 安装

**Kimi 桌面版（个人插件市场）**：

1. 克隆本仓库；
2. 让 agent 执行插件登记（`plugin-builder` 技能的 `register_personal` 流程），或在插件页「个人」页签按指引添加本目录；
3. 到「个人」页签点 ＋ 安装——免重启，当前会话即可用。

**手动（任意支持 SKILL.md 的 agent）**：把 `skills/context-handoff/` 复制到你的 skills 目录即可。

## 使用（自然语言）

- 「我要换窗口了，先写接续现场笔记」
- 「新会话，读接续笔记接手」
- 「刚才是不是压缩了？做一次回读验收」
- 「按装机清单核对一遍在位情况」

## 仓库结构

```
context-handoff/
├── kimi.plugin.json                 # 插件清单（Kimi 插件规范）
├── skills/
│   └── context-handoff/
│       └── SKILL.md                 # 规程正文（交五栏／接四步／清单核对／观测立档）
├── LICENSE                          # MIT
└── README.md
```

## English summary

**context-handoff** is a skill-only Kimi plugin that formalizes a battle-tested protocol for handing work across LLM context boundaries — compressions, window switches, cold starts. On the way out ("hand off"), the agent writes a five-section field note (current directive / done-list / frozen decisions / toolchain notes / open gaps) addressed to a zero-context successor. On the way in ("take over"), the new session runs a four-step intake: read the note and the single source-of-truth ledger, verify the install manifest, self-report its state, then **validate against artifacts, not self-narration** (git log, files on disk, registries). Every compression is archived as a numbered observation log. Iron rule: judgment and arbitration stay on the human side — no adapter layer may decide in the human's place. Born from a real session that survived a forced context compaction with zero work loss (observation log #001, 2026-08-28).

## License

MIT © 潘罗嘉 (luojia522)
