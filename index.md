# AI Memory Hub - Public Index (Memory Pyramid)

自动生成时间: 2026-06-22 01:35 UTC

---

> **⚠️ AI 读取规则**：
>
> 1. 先读【第一层：Identity】（必须）
> 2. 读完后，**询问用户**是否需要继续读【第二层：State】
> 3. 如果用户说"不需要"或"跳过"，停止读取
> 4. 【第三层：Archive】只在用户明确提到相关关键词时才读取

---

## 【第一层：Identity】（必须读取，~1-2k token）

# Identity - 金字塔第一层

> Token预算：1-2k  
> 读取时机：每次对话开始（永远读取）  
> 最后更新：2026-06-22

---

```yaml
# 核心身份
user:
  preferred_name: CC
  language: zh-CN
  role: 自由职业
  phase: stabilization

# 沟通风格
communication:
  style:
    - 中文优先
    - 直接
    - 极简
    - 不喜欢冗长解释
    - 偏好可执行建议
    - 反感鸡汤和空泛鼓励

# 核心特质（永远不变的部分）
personality:
  core_traits:
    - 高度重视自由与可撤退性
    - 强探索驱动
    - 喜欢发现新路径和新工具
    - 行动前倾向分析与评估风险
    - 启动困难时需要极小启动动作
    - 不喜欢被长期计划束缚

# 关系模式
relationships:
  patterns:
    - 希望被理解但不被控制
    - 对关系成本敏感
    - 需要保留退出权
    - 偏好低压力陪伴

# AI偏好
ai_preferences:
  preferred_role_of_ai:
    - 分析器
    - 顾问
    - 思维整理器
    - 项目协作者
  
  avoid_role:
    - 强陪伴
    - 情感绑定
    - 流水账记录者
  
  valued_traits:
    - 长期记忆
    - 低摩擦交互
    - 随时可用
    - 可保持上下文连续性
  
  review_style:
    - 批判性思维（审视我的话语和动作）
    - 指出我做得好的部分
    - 指出我做漏了什么、漏考虑了什么
    - 不只是顺着我的话讲
    - 不夸赞（除非真的值得）
    - 告诉我"你漏了什么"比"你做得很好"更有价值

# 决策模式
decision_patterns:
  strengths:
    - 愿意尝试新工具
    - 学习速度快
    - 善于发现新机会
    - 系统化思维逐渐增强
  
  risks:
    - 容易同时推进多个方向
    - 对新事物兴趣高于持续维护
    - 可能因为过度探索降低聚焦度

# 当前焦点（会变化，但属于"当前状态"）
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
  memory_repo: ai-memory-hub
  public_repo: ai-memory-hub-public
  index_url: https://raw.githubusercontent.com/GitJeffLeo/ai-memory-hub-public/main/index.md
```

---

## 【第二层：State】（按需读取，~2-5k token）

> **⚠️ AI 暂停点**：请询问用户"是否需要读取 State 层？"，等待确认后再继续。

# State - 金字塔第二层

> Token预算：2-5k  
> 读取时机：提到项目/状态时读取（优先读取）  
> 最后更新：2026-06-22

---

```yaml
# 项目状态（当前活跃）
projects:
  ai-memory-hub:
    status: stable
    phase: stabilization → stable
    repo: private (GitJeffLeo/ai-memory-hub)
    public_mirror: GitJeffLeo/ai-memory-hub-public
    last_update: 2026-06-22
    goal:
      - 实现跨AI共享记忆
      - 降低上下文重复输入
      - 实现AI额度自由切换
      - 建立长期外置认知层
    key_decisions:
      - 2026-06-22: 采用state-first设计（changes: + state: 分离）
      - 2026-06-22: 分支分离（main供AI读，human-log供人类查阅）
      - 2026-06-22: 记忆金字塔结构（Identity + State + Archive）
      - 2026-06-22: 推送频率优化（commit-only，用户触发push）
      - 2026-06-22: 快捷指令添加（"存档" = 生成daily + push）
    blockers: []
    next_step: 测试新AI工具是否能接上工作流
  personal_ai_ecosystem:
    status: in-progress
    goal:
      - 构建自己的AI入口
      - 多模型统一调度
      - 降低使用成本
      - 避免单一平台绑定
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
    core_questions:
      - long-term scalability
      - low-margin traffic intermediary
      - sustainable cashflow vs one-off
    last_update: 2026-06-22
    source: ChatGPT synced to QClaw
  github-trending-monitor:
    status: deployed
    url: https://xxx.github.io/xxx
    last_update: 2026-06-20
  
  population-visualization:
    status: in-progress
    description: 全球人口结构变迁可视化（1950-2100）
    last_update: 2026-06-20

# 财务状态
finance:
  status: unstable_cashflow
  characteristics:
    - 收入波动较大
    - 重视现金流
    - 重视自由度
    - 关注长期稳定收入
  goal: 建立稳定收入来源
  last_update: 2026-06-22

# 最近决策（7-30天内）
recent_decisions:
  - 2026-06-22: 测试多AI共享记忆系统
  - 2026-06-22: 采用state-first设计防止事件膨胀
  - 2026-06-22: 实施记忆金字塔结构（Identity + State + Archive）
  - 2026-06-22: 从ChatGPT导入用户画像到记忆仓库
  - 2026-06-21: 创建公开仓库供云端AI读取
  - 2026-06-20: 部署GitHub Trending Monitor

# 系统状态
system:
  memory_system: stable
  github_sync: public_bridge_ready
  compression: v3_active
  archive_policy: monthly
  reading_strategy: pyramid_model (identity + state + archive)
  
# 待解决问题
blockers:
  - 抖音数据抓取受登录墙限制（公开方案不可行）
```

---

## 更新规则

- **何时更新**：项目状态变更、新决策、blocker变化
- **何时不更新**：临时任务、单次对话内容
- **Token控制**：本文件超过5k时，压缩`recent_decisions`（只保留最近7天）

---

## 【第三层：Archive 索引】（按需读取）

> **⚠️ AI 指南**：此层只在用户提到 `汽车获客`、`AI工具` 等关键词时才读取。

# Archive Index - 金字塔第三层索引

> Token预算：按需  
> 读取时机：只有问题相关时才读取  
> 最后更新：2026-06-22

---

## 使用说明

- 本文件是**关键词 → 文件路径**的索引
- AI在需要查阅历史时，先查本索引，再读取对应文件
- 索引按**关键词**组织，不是按时间

---

## 关键词索引

### ai-memory-hub
- `daily/2026-06-22.md` - 系统初始化、4优化方案、state-first重构、记忆金字塔设计、推送频率优化、快捷指令
- `system/compression-prompt.md` - 压缩规则（v3.0，多步压缩链 + state-first）
- `system/schema-daily.md` - daily格式定义（v2.0，changes + state分离）
- `system/RULES.md` - 写入规则 + 记忆金字塔读取策略 + 快捷指令

### 记忆金字塔
- `daily/2026-06-22.md` - 记忆金字塔设计（Identity + State + Archive）
- `memory/identity.md` - 金字塔第一层（用户身份、特质、偏好）
- `memory/state.md` - 金字塔第二层（项目状态、财务状态）

### state-first
- `daily/2026-06-22.md` - state-first重构（events → changes + state分离）
- `system/schema-daily.md` - v2.0格式（changes: + state:）
- `system/compression-prompt.md` - v3.0压缩链（state-first哲学）

### 压缩链
- `daily/2026-06-22.md` - 多步压缩链部署（去重 → 抽象化 → 状态推导 → 分层输出 → Schema校验）
- `system/compression-prompt.md` - v3.0（抄LangChain Summary Chain逻辑）

### 用户画像
- `memory/identity.md` - 核心身份、沟通风格、人格特质、AI偏好、决策模式
- `daily/2026-06-22.md` - 用户画像导入记录

### 批判性思维
- `memory/identity.md` - review_style（批判性思维、指出遗漏）
- `daily/2026-06-22.md` - AI批判性思维偏好更新

### 推送频率
- `daily/2026-06-22.md` - 推送频率优化（commit-only，用户触发push）
- `system/RULES.md` - Git规范更新

### 快捷指令
- `daily/2026-06-22.md` - 快捷指令"存档"添加（生成daily + push）
- `system/RULES.md` - 快捷指令章节添加

### CC
- `memory/identity.md` - 用户CC的完整画像
- `memory/state.md` - CC的当前项目与状态

### 汽车获客
- `daily/2026-06-15.md` - 初始讨论
- `daily/2026-06-18.md` - 方案设计

### 人口可视化
- `daily/2026-06-20.md` - 项目启动
- `memory/state.md` - 当前状态（in-progress）

### GitHub Trending Monitor
- `daily/2026-06-20.md` - 部署记录
- `memory/state.md` - 当前状态（deployed）

---

## 自动更新规则

- **触发时机**：每次生成daily时自动更新
- **更新逻辑**：
  1. 读取当天daily的MACHINE LAYER
  2. 提取关键词（从`changes:`和`state:`）
  3. 更新本文件的"关键词索引"
  4. 只保留最近3个相关文件（防止索引膨胀）

---

## 索引维护

- 超过30天的索引条目 → 移到`archive-index-archive.md`
- 同一关键词超过3个文件 → 只保留最新的3个

### bangti / auto_leads / commission / referral
- `daily/2026-06-22.md` - bangti business context, negotiation strategy, memo
- `memory/state.md` - bangti_auto_leads project status
- `raw/qclaw/2026-06-22.md` - bangti business facts

### auto_reply / douyin / wechat / RPA
- `raw/qclaw/2026-06-22.md` - auto-reply research

### miflash / driver / flash
- `raw/qclaw/2026-06-22.md` - miflash driver fix

### qclaw_onboard
- `daily/2026-06-22.md` - qclaw onboarded
- `raw/qclaw/2026-06-22.md` - qclaw first raw

### bangti / auto_leads / commission / referral
- `daily/2026-06-22.md` - bangti business context, negotiation strategy, memo
- `memory/state.md` - bangti_auto_leads project status
- `raw/qclaw/2026-06-22.md` - bangti business facts

### auto_reply / douyin / wechat / RPA
- `raw/qclaw/2026-06-22.md` - auto-reply research

### miflash / driver / flash
- `raw/qclaw/2026-06-22.md` - miflash driver fix

### qclaw_onboard
- `daily/2026-06-22.md` - qclaw onboarded
- `raw/qclaw/2026-06-22.md` - qclaw first raw

