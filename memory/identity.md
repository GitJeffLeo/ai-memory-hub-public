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

# 变更溯源（记录关键字段最近一次更新的来源）
last_updated:
  review_style: {date: 2026-06-22, trigger: "raw/workbuddy/2026-06-22.md line 82", change: "添加批判性思维偏好"}
  current_focus: {date: 2026-06-22, trigger: "raw/workbuddy/2026-06-22.md line 73", change: "导入ChatGPT用户画像"}
```
