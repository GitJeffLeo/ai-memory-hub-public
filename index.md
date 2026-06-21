# AI Memory Hub - Public Index (State-Only)

自动生成时间: 2026-06-21 23:53 UTC

---

> ⚠️ 此文件为 AI 设计（state-only）。人类查阅请切换到 `human-log` 分支。

---

## memory/profile.md

# Profile (DEPRECATED)

> **状态**：已废弃（2026-06-22）  
> **替代文件**：`memory/identity.md`  
> **原因**：重构为记忆金字塔结构（Identity + State + Archive）

---

本文件内容已迁移至：
- 核心身份 → `memory/identity.md`
- 用户画像 → `memory/identity.md`

**不要删除本文件**（防止外部链接失效），但所有 AI 节点应读取 `memory/identity.md`。

---

## memory/projects.md

# Projects (DEPRECATED)

> **状态**：已废弃（2026-06-22）  
> **替代文件**：`memory/state.md`  
> **原因**：重构为记忆金字塔结构（Identity + State + Archive）

---

本文件内容已迁移至：
- 项目状态 → `memory/state.md`（projects: 字段）

**不要删除本文件**（防止外部链接失效），但所有 AI 节点应读取 `memory/state.md`。

---

## memory/preferences.md

# Preferences (DEPRECATED)

> **状态**：已废弃（2026-06-22）  
> **替代文件**：`memory/identity.md`  
> **原因**：重构为记忆金字塔结构（Identity + State + Archive）

---

本文件内容已迁移至：
- AI生态 → `memory/identity.md`（ai_ecosystem: 字段）
- 沟通偏好 → `memory/identity.md`（communication: 字段）

**不要删除本文件**（防止外部链接失效），但所有 AI 节点应读取 `memory/identity.md`。

---

## Latest Daily State (from 2026-06-22)

# Daily Memory - 2026-06-22

## MACHINE LAYER

```yaml
project_status: infra_ready → stabilization
events:
  - ai-memory-hub: initialized (private repo, 3-layer, 7 sources)
  - dual_layer_format: adopted → upgraded to machine-layer-only
  - memory_compression_v1: deployed
  - workbuddy_raw_log: created (raw/workbuddy/2026-06-22.md)
  - system_rules: updated (daily trigger = ask user each turn)
  - deduplication_rules: defined (system/dedup-rules.md)
  - memory_trigger_rules: defined (only on fundamental state change)
  - human_layer: disabled in daily (on-demand restoration via system/restore-human-layer.md)
  - monthly_report: planned (30-day compression + raw archive)
  - public_sync: planned (github actions → public repo for cloud AI access)
blockers:
  - chatgpt: cannot access private github repo (pending public repo setup)
  - douyin_data: requires app or third-party platform login
  - cloud_ai_autonomous_read: blocked by private repo (solution: public repo + github actions)
state: system built, rules clarified, entering stable operation
```

