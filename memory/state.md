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
