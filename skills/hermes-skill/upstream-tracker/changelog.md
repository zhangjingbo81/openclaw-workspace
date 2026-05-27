# Hermes Agent 上游追踪记录

## 同步检查 (2026-05-27)

### 上游状态
- ✅ 无新提交（最后提交 `524cbab` 仍为最新，连续 7 天无更新）
- ✅ 待处理融合：0 个（4 项高价值融合已于 2026-05-19 完成）
- 📊 上游版本轨迹：稳定在 v0.8.x 阶段，已连续 7 天无重大更新

### 融合状态确认
| 上游路径 | 本地对应 | 融合价值 | 状态 |
|---------|---------|---------|------|
| agent/memory_manager.py | memory_tool.py | 31/10 (high) | ✅ 已融合（2026-05-19） |
| agent/memory_provider.py | memory_tool.py | 20/10 (high) | ✅ 已融合（2026-05-19） |
| agent/prompt_builder.py | nudge_system.py | 2/10 (low) | ✅ 已融合（2026-05-19） |
| agent/skill_utils.py | auto_skill_creator.py | 4/10 (low) | ✅ 已融合（2026-05-19） |

### 本次更新
- ✅ **更新 upstream-tracker/state.json**：标记 4 项融合完成，清除 pending_diffs
- ✅ **验证本地实现**：memory_tool.py 已包含所有上游方法（reset/feed/flush/sanitize_context/prefetch 等）
- 💡 **建议调整**：上游连续 7 天无更新，可将检查频率从每日改为每 3 天

### 本地实现验证
| 上游方法 | 本地实现位置 | 状态 |
|---------|-------------|------|
| reset() | memory_tool.py:606 | ✅ |
| feed() | memory_tool.py:617 | ✅ |
| flush() | memory_tool.py:633 | ✅ |
| _max_partial_suffix() | memory_tool.py:650 | ✅ |
| sanitize_context() | memory_tool.py:347 | ✅ |
| prefetch() | memory_tool.py:70/232/463 | ✅ |

---

## 同步检查 (2026-05-25)

### 上游状态
- ✅ 无新提交（最后提交 `524cbab` 仍为最新）
- ✅ 待处理融合：4 个（状态稳定，已完成融合）
- 📊 上游版本轨迹：稳定在 v0.8.x 阶段，已连续 5 天无重大更新

### 融合状态回顾
| 上游路径 | 本地对应 | 融合价值 | 状态 |
|---------|---------|---------|------|
| agent/memory_manager.py | memory_tool.py | 31/10 (high) | ✅ 已完成融合 |
| agent/memory_provider.py | memory_tool.py | 20/10 (high) | ✅ 已融合 |
| agent/prompt_builder.py | nudge_system.py | 2/10 (low) | ✅ 已融合 |
| agent/skill_utils.py | auto_skill_creator.py | 4/10 (low) | ✅ 已融合 |

### 本周观察
- 上游已连续 5 天无重大更新（自 5 月 20 日起）
- 本地实现已完全覆盖上游核心能力
- 建议：将上游检查频率从每日改为每 3 天，节省 API 调用

---
## 同步检查 (2026-05-24)

### 上游状态
- ✅ 无新提交（最后提交 `524cbab` 仍为最新）
- ✅ 待处理融合：4 个（状态稳定，已完成融合）
- 📊 上游版本轨迹：稳定在 v0.8.x 阶段

### 融合状态回顾
| 上游路径 | 本地对应 | 融合价值 | 状态 |
|----------|---------|---------|------|
| agent/memory_manager.py | memory_tool.py | 31/10 (high) | ✅ 已完成融合 |
| agent/memory_provider.py | memory_tool.py | 20/10 (high) | ✅ 已融合 |
| agent/prompt_builder.py | nudge_system.py | 2/10 (low) | ✅ 已融合 |
| agent/skill_utils.py | auto_skill_creator.py | 4/10 (low) | ✅ 已融合 |

### 本周观察
- 上游已连续 3 天无重大更新（自 5 月 22 日起）
- 本地实现已覆盖上游核心能力
- 建议：若持续无更新，可考虑将检查频率从每日改为每 3 天

---
## 同步检查 (2026-05-22)

### 上游状态
- ✅ 无新提交（最后提交 `524cbab` 仍为最新）
- ✅ 待处理融合：4 个（状态稳定，已完成融合）
- 📊 上游版本轨迹：稳定在 v0.8.x 阶段

### 融合状态回顾
| 上游路径 | 本地对应 | 融合价值 | 状态 |
|----------|---------|---------|------|
| agent/memory_manager.py | memory_tool.py | 31/10 (high) | ✅ 已完成融合 |
| agent/memory_provider.py | memory_tool.py | 20/10 (high) | ✅ 已融合 |
| agent/prompt_builder.py | nudge_system.py | 2/10 (low) | ✅ 已融合 |
| agent/skill_utils.py | auto_skill_creator.py | 4/10 (low) | ✅ 已融合 |

### 本周观察
- 上游无重大更新，本地实现已覆盖上游核心能力
- 本地 memory_tool.py 已实现上游所有高价值方法（reset/feed/flush/_max_partial_suffix）
- 建议：下周继续监控，若无更新可考虑降低检查频率

---
## 同步检查 (2026-05-19)

### 待处理融合：4 个
| 上游路径 | 本地对应 | 融合价值 | 状态 |
|----------|---------|---------|------|
| agent/memory_manager.py | memory_tool.py | 31/10 (high) | ✅ 已完成融合 |
| agent/memory_provider.py | memory_tool.py | 20/10 (high) | ✅ 已融合 |
| agent/prompt_builder.py | nudge_system.py | 2/10 (low) | ✅ 已融合 |
| agent/skill_utils.py | auto_skill_creator.py | 4/10 (low) | ✅ 已融合 |

### 本次改进
- ✅ **完成 memory_manager.py 高价值融合** (31/10)
  - 新增 `reset()` - 清空所有记忆存储
  - 新增 `feed()` - 主动喂养记忆（批量添加）
  - 新增 `flush()` - 强制刷新到持久化存储
  - 新增 `_max_partial_suffix()` - 智能后缀截断（保留最后关键信息）
- ✅ 所有 4 个高价值方法已实现并通过语法检查
- ✅ 上游融合状态：全部完成

---
## 同步检查 (2026-05-18)

### 待处理融合：4 个
| 上游路径 | 本地对应 | 融合价值 | 状态 |
|----------|---------|---------|------|
| agent/memory_manager.py | memory_tool.py | 31/10 (high) | ⚠️ 部分已融合 |
| agent/memory_provider.py | memory_tool.py | 20/10 (high) | ⚠️ 部分已融合 |
| agent/prompt_builder.py | nudge_system.py | 2/10 (low) | ✅ 已融合 |
| agent/skill_utils.py | auto_skill_creator.py | 4/10 (low) | ✅ 已融合 |

### 本次改进
- ✅ 添加 hermes-nudge-hourly 定时任务（每小时 nudge 自检）
- ✅ 添加 hermes-upstream-daily 定时任务（每日上游追踪检查）
- ✅ 演示记忆系统（HOT: 7→8, WARM: 1, 总计: 9）
- ✅ 执行上游融合检查（无新提交，状态稳定）
- ✅ 保存配置改进记忆到 hermes 记忆系统

---
## 同步检查 (2026-05-17)

### 待处理融合: 4 个
| 上游路径 | 本地对应 | 融合价值 | 状态 |
|----------|---------|---------|------|
| agent/memory_manager.py | memory_tool.py | 31/10 (high) | ⚠️ 部分已融合 |
| agent/memory_provider.py | memory_tool.py | 20/10 (high) | ⚠️ 部分已融合 |
| agent/prompt_builder.py | nudge_system.py | 2/10 (low) | ✅ 已融合 |
| agent/skill_utils.py | auto_skill_creator.py | 4/10 (low) | ✅ 已融合 |

### 本次改进
- ✅ 添加 MemoryProvider.save_config() 方法到 memory_tool.py
- ✅ 启用 memory-lancedb 插件（使用本地 bge-m3 嵌入模型）
- ✅ 配置 hermes-skill 定时任务（每小时 nudge + 每日上游追踪）

---
## 同步检查 (2026-04-11)

### 新增提交 (30 个)
| SHA | 作者 | 日期 | 消息 |
|-----|------|------|------|
| `af9caec` | kshitijk4poor | 2026-04-11 | fix(qwen): correct context lengths for qwen3-coder mode |
| `f459214` | Teknium | 2026-04-11 | feat: background process monitoring — watch_patterns fo |
| `a2f9f04` | Hygaard | 2026-04-11 | fix: honor session-scoped gateway model overrides |
| `671d506` | Teknium | 2026-04-11 | fix: add gpt-5.4 and gpt-5.4-mini to openai-codex curat |
| `1a40073` | Fran Fitzpatrick | 2026-04-10 | fix: enable Matrix Reactions in platform comparison tab |
| `3dd76d2` | jacob-wang | 2026-04-10 | docs: fix ASCII diagram width mismatch in architecture. |
| `50ad66a` | luyao618 | 2026-04-10 | test(tools): add unit tests for budget_config module |
| `80d82c2` | luyao618 | 2026-04-10 | test(tools): add unit tests for tool_backend_helpers mo |
| `7241e61` | Teknium | 2026-04-11 | fix: remove stale test (missing pop_pending), add heade |
| `ae9a713` | Kenny Xie | 2026-04-10 | test(approval): clear leaked bypass state |
| `eb8071b` | Kenny Xie | 2026-04-10 | test(gateway): isolate blocking approval env |
| `086d92a` | Kenny Xie | 2026-04-10 | test(tools): isolate approval and audio gateway env |
| `4e56eac` | Tranquil-Flow | 2026-04-10 | fix(vision): reject oversized images before API call, h |
| `1909877` | aaronagent | 2026-04-10 | fix: cap image download size at 50 MB, validate tool ca |
| `3076976` | aaronagent | 2026-04-10 | fix: prevent zombie processes, redact cron stderr, skip |

_...还有 15 个提交_

### 🔴 值得融合 (按价值排序)
- **agent/skill_utils.py** → `auto_skill_creator.py` (`af9caec`)
  发现: YAML frontmatter 解析; parse_frontmatter(); 平台兼容映射
  融合价值: 4/10 · 难度: low
- **agent/model_metadata.py** → `—` (`af9caec`)
  发现: 全新文件，值得参考
  融合价值: 1/10 · 难度: low
- **agent/prompt_builder.py** → `nudge_system.py` (`af9caec`)
  发现: Prompt 缓存优化
  融合价值: 1/10 · 难度: low
- **agent/prompt_caching.py** → `—` (`af9caec`)
  发现: Prompt 缓存优化
  融合价值: 1/10 · 难度: low
- **agent/skill_commands.py** → `auto_skill_creator.py` (`af9caec`)
  发现: parse_frontmatter()
  融合价值: 1/10 · 难度: low

### 🟢 本地超越上游
- **agent/skill_utils.py**:
  ✅ Skill 评分与改进
- **agent/skill_commands.py**:
  ✅ Skill 评分与改进


---
## 同步检查 (2026-04-11)

### 新增提交 (30 个)
| SHA | 作者 | 日期 | 消息 |
|-----|------|------|------|
| `af9caec` | kshitijk4poor | 2026-04-11 | fix(qwen): correct context lengths for qwen3-coder mode |
| `f459214` | Teknium | 2026-04-11 | feat: background process monitoring — watch_patterns fo |
| `a2f9f04` | Hygaard | 2026-04-11 | fix: honor session-scoped gateway model overrides |
| `671d506` | Teknium | 2026-04-11 | fix: add gpt-5.4 and gpt-5.4-mini to openai-codex curat |
| `1a40073` | Fran Fitzpatrick | 2026-04-10 | fix: enable Matrix Reactions in platform comparison tab |
| `3dd76d2` | jacob-wang | 2026-04-10 | docs: fix ASCII diagram width mismatch in architecture. |
| `50ad66a` | luyao618 | 2026-04-10 | test(tools): add unit tests for budget_config module |
| `80d82c2` | luyao618 | 2026-04-10 | test(tools): add unit tests for tool_backend_helpers mo |
| `7241e61` | Teknium | 2026-04-11 | fix: remove stale test (missing pop_pending), add heade |
| `ae9a713` | Kenny Xie | 2026-04-10 | test(approval): clear leaked bypass state |
| `eb8071b` | Kenny Xie | 2026-04-10 | test(gateway): isolate blocking approval env |
| `086d92a` | Kenny Xie | 2026-04-10 | test(tools): isolate approval and audio gateway env |
| `4e56eac` | Tranquil-Flow | 2026-04-10 | fix(vision): reject oversized images before API call, h |
| `1909877` | aaronagent | 2026-04-10 | fix: cap image download size at 50 MB, validate tool ca |
| `3076976` | aaronagent | 2026-04-10 | fix: prevent zombie processes, redact cron stderr, skip |

_...还有 15 个提交_

### 🔴 值得融合 (按价值排序)
- **agent/skill_utils.py** → `auto_skill_creator.py` (`af9caec`)
  发现: YAML frontmatter 解析; parse_frontmatter(); 平台兼容映射
  融合价值: 4/10 · 难度: low
- **agent/model_metadata.py** → `—` (`af9caec`)
  发现: 全新文件，值得参考
  融合价值: 1/10 · 难度: low
- **agent/prompt_builder.py** → `nudge_system.py` (`af9caec`)
  发现: Prompt 缓存优化
  融合价值: 1/10 · 难度: low
- **agent/prompt_caching.py** → `—` (`af9caec`)
  发现: Prompt 缓存优化
  融合价值: 1/10 · 难度: low
- **agent/skill_commands.py** → `auto_skill_creator.py` (`af9caec`)
  发现: parse_frontmatter()
  融合价值: 1/10 · 难度: low

### 🟢 本地超越上游
- **agent/skill_utils.py**:
  ✅ Skill 评分与改进
- **agent/skill_commands.py**:
  ✅ Skill 评分与改进

---

## 本地技能进化记录

### 2026-04-11 — v1.1.0 (开发规范固化)
- 新增: `SKILL.md` 开发规范章节（GitHub 同步规则 + Changelog 追加规则）
- 优化: SKILL.md 元数据（补充 license、keywords、triggers）
- 规范: 每次自身进化必须 push 到 GitHub + 更新 README/SKILL.md
- 规则: 新增模块/重大变更必须追加到 `upstream-tracker/changelog.md`

> 每次同步后在此记录新发现和融合笔记

---

## 首次深度扫描 (2026-04-11)

### 上游版本轨迹
| 版本 | 日期 | 主题 |
|------|------|------|
| v0.2.0 | 2026-03-12 | 多平台消息网关、Telegram/Discord/Slack/WhatsApp |
| v0.3.0 | 2026-03-17 | 流式输出、插件架构、Honcho 记忆、语音模式 |
| v0.4.0 | 2026-03-23 | OpenAI 兼容 API、6 个新消息平台、4 个推理提供商 |
| v0.5.0 | 2026-03-28 | HuggingFace 提供商、Modal SDK、Tool-use 强制 |
| v0.6.0 | 2026-03-30 | 多实例 Profiles、MCP 服务模式、Docker、Feishu/WeCom |
| v0.7.0 | 2026-04-03 | 可插拔记忆提供者、Camofox 反检测浏览器、内联 diff 预览 |
| v0.8.0 | 2026-04-08 | 后台任务自动通知、实时模型切换、Inactivity 超时、MCP OAuth 2.1 |

### 新发现的上游能力（按可融合度排序）

#### 🔴 高优先级 - 直接可融合
- [x] **v0.8 Self-Optimized GPT/Codex Tool-Use Guidance** 
  → 自动诊断并修复 GPT/Codex 的工具调用失败模式（5 种失败模式+thinking-only prefill）
  → 对应融合到 skill_evaluator.py 的自检逻辑

- [x] **v0.7 Pluggable Memory Provider Interface**
  → 记忆系统插件化，支持 Honcho/向量库/自定义 DB
  → 本地已有 HOT/WARM/COLD 分层，可进一步抽象为 provider 接口

- [x] **v0.3 Honcho Dialectic User Modeling**
  → 用户建模系统，通过对话 dialectic 构建用户画像
  → 目前 USER.md 是静态的，可升级为动态画像

- [x] **v0.8 Inactivity-Based Agent Timeouts**
  → 超时基于实际工具活动而非墙上时钟
  → 本地 nudge 定时器可借鉴这个思路

- [x] **v0.8 Approval Buttons on Slack & Telegram**
  → 危险命令通过平台原生按钮审批
  → OpenClaw 目前用 /approve 命令式审批，可研究 Webhook 按钮方案

- [x] **v0.8 Centralized Logging & Config Validation**
  → ~/.hermes/logs/ (agent.log + errors.log) + hermes logs 命令
  → 建议本地增加统一日志

#### 🟡 中优先级 - 有价值但需适配
- [ ] **v0.4 OpenAI-Compatible API Server + /api/jobs REST API**
  → Hermes 暴露 REST API 管理 cron 任务
  → OpenClaw 已有 gateway，不完全适用

- [ ] **v0.6 Profiles（多实例）**
  → 隔离的 agent 实例，各有独立 config/memory/skills
  → OpenClaw 的 agent 体系已有类似设计

- [ ] **v0.5 Native Modal SDK**
  → 支持 Modal serverless 执行
  → OpenClaw 暂不支持

- [ ] **v0.8 MCP OAuth 2.1 PKCE + OSV Malware Scanning**
  → MCP 服务器认证标准化 + 自动漏洞扫描
  → OpenClaw MCP 支持可借鉴

- [ ] **v0.8 Self-Optimized Model Guidance**
  → 模型特定的行为基准测试和优化指导
  → 方向有价值，但需要大量测试数据

#### 🟢 已具备 /