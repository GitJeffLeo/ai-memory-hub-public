# State - 金字塔第二层

> Token预算：2-5k  
> 读取时机：提到项目/状态时读取（优先读取）  
> 最后更新：2026-06-23

---

```yaml
# 当前焦点
current_focus:
  - ai-memory-hub
  - 多AI协同工作流
  - AI工具生态探索
  - 汽车获客与自媒体变现
  - 建立稳定收入来源

# AI生态（稳定配置）
ai_ecosystem:
  local_rw: [WorkBuddy, Qoder, Qclaw, Claude Code]
  cloud_ro: [ChatGPT, Claude, DeepSeek]
  memory_protocol: ai-memory-hub (github-based)

# 系统原则
system_principles:
  - 记忆独立于模型
  - AI可替换
  - 状态比事件重要
  - 压缩优于堆积
  - 优先保留长期有效信息

# 系统配置
system:
  memory_repo: ai-memory-hub (private)
  memory_system: stable
  compression: v4_active (outcome-first)
  reading_strategy: pyramid_model (identity + state + archive)

# 项目状态（当前活跃）
projects:
  ai-memory-hub:
    status: stable
    repo: private (GitJeffLeo/ai-memory-hub)
    public_mirror: GitJeffLeo/ai-memory-hub-public
    last_update: 2026-06-23
    purpose: 记忆接力——切换AI时同步上下文，非多AI实时协作
    key_decisions:
      - 当前使用的AI即为写入方
      - 平时本地记录，切换AI时才push
      - 记忆金字塔（Identity + State + Archive）
      - 快捷指令（保存/存档/读档）
    blockers: []
    next_step: 将启动配置注入其他AI（Claude Code/QClaw/WorkBuddy）
  personal_ai_ecosystem:
    status: in-progress
    goal: [构建自己的AI入口, 多模型统一调度, 降低使用成本, 避免单一平台绑定]
    last_update: 2026-06-22
  bangti_auto_leads:
    status: negotiation
    phase: validation
    model: content_traffic_to_lead_to_referral_to_commission
    role: traffic acquisition + customer touchpoint
    leads_count: ~9
    current_focus: commission rules and settlement terms
    key_risks:
      - client ownership clarity (risk of bypass)
      - commission settlement cycle and delay
      - deal transparency (price manipulation)
      - traffic ownership control
      - first deal clean close
    last_update: 2026-06-22
  github-trending-monitor:
    status: deployed
    last_update: 2026-06-20
  population-visualization:
    status: in-progress
    description: 全球人口结构变迁可视化（1950-2100）
    last_update: 2026-06-20

# 财务状态
finance:
  status: unstable_cashflow
  characteristics: [收入波动较大, 重视现金流, 重视自由度]
  goal: 建立稳定收入来源
  last_update: 2026-06-22

# 待解决问题
blockers:
  - 抖音数据抓取受登录墙限制（公开方案不可行）

# 变更溯源
last_updated:
  bootstrap: {date: 2026-06-23, change: "创建BOOTSTRAP.md启动协议+精简架构为Qoder单写入方模式"}
  identity_optimization: {date: 2026-06-23, change: "identity.md精简至~1k token，可变内容迁入state.md"}
  simplification: {date: 2026-06-23, change: "移除CI/去重/多schema/月报等过度设计，保留最小可用架构"}
  ai-memory-hub: {date: 2026-06-22, trigger: "raw/workbuddy/2026-06-22.md", change: "状态标记为stable"}
  bangti_project: {date: 2026-06-22, trigger: "raw/qclaw/2026-06-22.md", change: "帮提谈判准备完成"}
  finance: {date: 2026-06-22, trigger: "raw/workbuddy/2026-06-22.md", change: "导入ChatGPT财务状态"}
```

---

## 更新规则

- **何时更新**：项目状态变更、新决策、blocker变化
- **何时不更新**：临时任务、单次对话内容
- **Token控制**：本文件超过5k时，压缩recent_decisions（只保留最近7天）
