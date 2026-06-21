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
- `daily/2026-06-22.md` - 系统初始化、state-first重构、记忆金字塔设计
- `system/compression-prompt.md` - 压缩规则（v3.0）
- `system/schema-daily.md` - daily格式定义（v2.0）
- `system/RULES.md` - 写入规则 + 记忆金字塔读取策略

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
