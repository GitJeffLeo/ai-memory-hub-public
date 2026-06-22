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
- `daily/2026-06-22.md` - 系统初始化、4优化方案、state-first重构、记忆金字塔设计、推送频率优化、快捷指令、按AI节点分组格式
- `system/compression-prompt.md` - 压缩规则（v3.0，多步压缩链 + state-first）
- `system/schema-daily.md` - daily格式定义（v3.0，按AI节点分组 + tags）
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

### ci_validation / format_drift
- `daily/2026-06-22.md` - CI validate.yml + raw/daily/memory 格式校验 + 格式漂移修正
- `.github/workflows/validate.yml` - CI 自动校验 workflow
- `system/schema-daily.md` - v3.0 tags 字段

### archive_checklist / tags / traceability
- `daily/2026-06-22.md` - 存档检查清单 + 标签体系 + 版本溯源
- `system/archive-checklist.md` - 6 步存档检查清单
- `system/schema-daily.md` - v3.0 12 标签封闭集合
- `memory/identity.md` - last_updated 溯源字段
- `memory/state.md` - last_updated 溯源字段

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

### Claude Code / claudecode
- `daily/2026-06-22.md` - Claude Code onboarded, write capability verified
- `raw/claudecode/2026-06-22.md` - Claude Code first raw log

### bangti / auto_leads / commission / referral
- `daily/2026-06-22.md` - bangti business context, negotiation strategy, memo
- `memory/state.md` - bangti_auto_leads project status
- `raw/qclaw/2026-06-22.md` - bangti business facts

### auto_reply / douyin / wechat / RPA
- `raw/qclaw/2026-06-22.md` - auto-reply research

### miflash / driver / flash
- `raw/qclaw/2026-06-22.md` - miflash driver fix

### shadowbot / uninstall / rpa
- `daily/2026-06-22.md` - ShadowBot 彻底卸载（进程/启动项/安装目录/用户数据/注册表/快捷方式）
- `raw/qclaw/2026-06-22.md` - 卸载详细步骤

### elevated_tools / uac / tools.elevated
- `daily/2026-06-22.md` - 开启 tools.elevated 配置（webchat 渠道 UAC 提权）
- `raw/qclaw/2026-06-22.md` - 配置修改详情

### shortcut_overlay / arrow / registry
- `daily/2026-06-22.md` - 去除快捷方式箭头角标（注册表 Shell Icons→29 + 计划任务自动修复）
- `raw/qclaw/2026-06-22.md` - 修复脚本和计划任务详情

### 读档 / pull / shortcut_commands
- `daily/2026-06-22.md` - 添加"读档"快捷指令（从 GitHub 拉取最新记忆）
- `MEMORY.md` - 快捷指令定义（存档/读档/推送/拉取）
