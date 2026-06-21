# Identity - 金字塔第一层

> Token预算：1-2k  
> 读取时机：每次对话开始（永远读取）  
> 最后更新：2026-06-22

---

```yaml
# 核心身份
user:
  name: CC
  language: zh-CN
  role: multi_ai_power_user
  phase: stabilization

# 核心特质（永远不变的部分）
traits:
  - 自由度优先
  - 探索驱动
  - 强调可撤退性
  - 直接执行，不列选项
  - 反感过度安全提醒

# 当前焦点（会变化，但属于"当前状态"）
current_focus:
  - ai-memory-hub
  - 汽车获客

# AI生态（稳定配置）
ai_ecosystem:
  local_rw: [WorkBuddy, Qoder, Qclaw, Claude Code]
  cloud_ro: [ChatGPT, Claude, DeepSeek]
  memory_protocol: ai-memory-hub (github-based)

# 沟通偏好（稳定）
communication:
  language: zh-CN
  tone: direct_minimal
  format: execute_first
  context_sharing: memory_feed_to_cloud

# 系统配置
system:
  memory_repo: ai-memory-hub
  public_repo: ai-memory-hub-public
  index_url: https://raw.githubusercontent.com/GitJeffLeo/ai-memory-hub-public/main/index.md
```
