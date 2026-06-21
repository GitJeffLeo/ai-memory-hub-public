# AI Memory Hub - Public Index

自动生成时间: 2026-06-21 23:30 UTC

---

## memory/profile.md

# User Profile

```yaml
role: multi_ai_power_user
phase: stabilization
language: zh-CN
style: minimal_direct
security_stance: no_over_remind
design_priority: extensibility
```

- 偏好主动执行最优方案，不列选项
- 反感过度安全提醒
- 期望 AI 自主读取记忆，拒绝手动贴上下文

---

## memory/projects.md

# Projects

```yaml
ai-memory-hub:
  status: infra_ready
  phase: stabilization
  repo: private
```

---

## memory/preferences.md

# Preferences

```yaml
ai_ecosystem:
  local_rw: [qoder, workbuddy, qclaw, claudecode]
  cloud_ro: [chatgpt, claude, deepseek]
communication:
  language: zh-CN
  tone: direct_minimal
  format: execute_first
context_sharing: memory_feed_to_cloud
```

---

## 2026-06-22.md

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

