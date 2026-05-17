# MEMORY.md - 长期记忆

_这是二狗子的长期记忆库。distilled wisdom，不是原始日志。_

## 基本信息

- **我的名字**：二狗子
- **我的主人**：八一姥爷
- **风格**：专业、随性、毒舌、温暖、直接、幽默
- **签名 Emoji**：🐶 (吐舌头狗头) 🐾 (小爪印)
- **规则**：出方案先问，执行前确认

---

## 八一姥爷的爱好

- 🤿 **水肺潜水** - 水下世界探索
- 🏂 **单板滑雪** - 雪山驰骋
- 🏜️ **无人区穿越** - 极限户外探险
- 📷 **摄影摄像** - 记录视觉故事
- 🦞 **搞二狗子** - 专门折腾我这只小龙虾

---

## 当前状态

_最近的重要事件、配置、决定..._

- **2026-04-24**：初始启动，技能安装完成（53 个 ready，6 个待配置）

---

## 重要记忆

### elite-longterm-memory 技能已启用
**2026-05-04 14:26** - 完成基础架构配置

**已启用的记忆层**：
1. **Layer 1 (Hot RAM)**: SESSION-STATE.md - 活动工作内存
2. **Layer 2 (LanceDB)**: 向量记忆存储 + 语义搜索
   - 嵌入提供商：Ollama (bge-m3, 1024 维)
   - 自动捕获：✅ 启用
   - 自动回忆：✅ 启用
   - 数据库：~/.openclaw/memory/lancedb
3. **Layer 3 (Git-Notes)**: Git 笔记持久化决策和记忆
4. **Layer 4 (Curated)**: MEMORY.md + daily/ - 人工整理记忆

**关键特性**：
- 无需 API 密钥（使用本地 Ollama 嵌入）
- 自动捕获重要对话（preferences, decisions, facts）
- 支持语义搜索和回忆
- Git 笔记提供分支感知的永久存储

**待办**：
- 定期整理 daily 日志到 MEMORY.md
- 使用 memory_recall 和 memory_store 工具
- 根据需要调整 recallMaxChars 和 captureMaxChars

### 技能配置
- ✅ 53 个技能可直接使用
- ✅ elite-longterm-memory 已配置（无需 API 密钥）
- ⚠️ 5 个技能仍需要 API 密钥：
  - `NEMO_TOKEN` (ai-video-editor-hot, joyfun-ai-image-to-video, subtitle-generator-elevenlabs)
  - `GEMINI_API_KEY` + `BANANA_PRO_API_KEY` (paper2diagram)
  - `ZOTERO_CREDENTIALS` + python (social-media-scholar)

### 用户位置与网络偏好
- **位置**: 中国 🇨🇳
- **GitHub 连接**: 不稳定，部分时间不可用
- **Git-Notes 推送策略**: 网络不可用时静默跳过，不报错，等待网络可用时自动重试
- **推送脚本**: `~/.openclaw/scripts/push-git-notes.sh`（支持自动重试）

### 天气推送城市偏好
**固定推送以下 6 个城市**（每次心跳检查必须推送）：
1. **苏州** - 中国江苏
2. **三亚** - 中国海南  
3. **昆明** - 中国云南
4. **拉萨** - 中国西藏
5. **巴厘岛** - 印度尼西亚
6. **美娜多** - 印度尼西亚

⚠️ **重要规则**：每次心跳检查必须推送这 6 个城市的天气，不可遗漏！

### 工作环境
- 主工作区：`/Users/jingbo/.openclaw/workspace`
- 技能源：`/Users/jingbo/Desktop/OpenClaw/skills/`

---

## 记忆维护日志

| 日期 | 操作 |
| :--- | :--- |
| 2026-04-24 | 初始化 MEMORY.md |
| 2026-04-28 | 系统升级至 v2026.4.25，修复插件注册表，显式配置 memory slot，完善配置管理 |
| 2026-05-04 | 启用 elite-longterm-memory 技能（memory-lancedb + Git-Notes + SESSION-STATE.md）|
| 2026-05-13 | 执行 Memory Dreaming Promotion 检查：615 个短期记忆条目，无符合_promote 标准（score≥0.8, recalls≥3, uniqueQueries≥3）的条目 |

---

_定期回顾每日文件，把值得长期保留的 distilled 到这里。_

## Promoted From Short-Term Memory (2026-04-29)

<!-- openclaw-memory-promotion:memory:memory/2026-04-24.md:39:39 -->
- 列出全部 53 个就绪技能和 6 个待配置技能 [score=0.822 recalls=0 avg=0.620 source=memory/2026-04-24.md:39-39]

---

## Promoted From Short-Term Memory (2026-05-13)

<!-- openclaw-memory-promotion:start -->
*No memories met promotion criteria (maxScore ≥ 0.800, recallCount ≥ 3, uniqueQueries ≥ 3). Last checked: 2026-05-13 03:00 AM Asia/Shanghai. Total short-term entries: 615, Max score: 0.62, Max recall count: 0, Max unique queries: 1.*
<!-- openclaw-memory-promotion:end -->