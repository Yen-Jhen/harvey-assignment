# 來源 03：AI 系統架構（審核後摘錄）

- 原始來源：Harvey 的 `context/ai-system.md`，文件所述架構提出於 2026-10-30。
- 整理日期：2026-11-15。
- 性質：下列為挑選的英文原文片段，**不是完整原始文件**；原始文件保留於原位。
- 範圍：只納入已確認的通用架構與工作原則。

## 背景與角色

> Persistent written context lives in plain Markdown and Git history, *not solely in chats*.

> Avoid one enormous all-purpose prompt. Keep small role instructions and load project context only when relevant.

> The user remains final scientific authority, responsible for manual data validation and production execution.

> ## Initial model roles (flexible hypotheses)

## 獨立驗證與交接

> Never assume multi-model agreement equals correctness. Models should independently check against **external references, toy results, invariants and known limits**.

> A local Git repo is a common file store and history, not a cross-provider chat bus.

> A conversation needs an upload, connector, compatible local file tool, or deliberate handoff to read repository files.

## 有界改善

> Upgrade only when there is a repeated failure, concrete need, or useful measurable opportunity.

> Define a small deliverable and acceptance criterion.

> Implement one bounded change; review the diff.

> Adopt, revise or discard. Record date and rationale.
