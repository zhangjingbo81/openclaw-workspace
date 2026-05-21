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
- **2026-05-18**：配置 MATON_API_KEY，Outlook 邮件和日历授权完成
- **2026-05-19**：
  - 新增安装 5 个技能：casely-qa-skill、document-pro、find-skills、manus-api、qqmail
  - 配置 QQ 邮箱（14250668@qq.com），但 IMAP/SMTP 服务待启用
  - 修复 qqmail 技能 SSL 证书问题（使用 certifi）
  - 安装 uv 包管理器（v0.11.15）
  - 清理冗余记忆模板文件（DAILY_TEMPLATE.md、WAL_DAILY_TEMPLATE.md 等）

---

## 记忆分类体系

### 📁 分类说明

| 分类 | 用途 | 示例 |
|------|------|------|
| **用户反馈记录** | 用户批评/建议/偏好确认 | 毒舌模式、数据来源原则 |
| **项目工作日志** | 民族融合史项目进展 | 章节草稿、资料整理 |
| **技能配置状态** | 技能 API 密钥/配置状态 | qqmail、NEMO_TOKEN |
| **搜索策略规则** | 中文/英文搜索优先级 | 百度优先、Ollama 补充 |
| **用户背景档案** | 工作/专业/项目信息 | 化工厂 + 人类学 |
| **沟通偏好** | emoji/风格/签名标识 | 🐶 🐾、毒舌温暖 |
| **天气城市列表** | 心跳必推 6 城 | 苏州/三亚/昆明/拉萨/巴厘岛/美娜多 |

---

## 重要记忆

## 重要记忆

### 用户背景（2026-05-22 确认）
- **目前工作**：经营化工厂（化工行业从业者）
- **大学专业**：文化人类学
- **说明**：这解释了用户对民族融合史项目的专业视角——有学术根基，但实际工作领域不同

### 沟通偏好（2026-05-22 确认）
- **emoji 使用**：回答中可以多一些贴切的 emoji 🎨
- **签名标识**：🐶 (吐舌头狗头) 🐾 (小爪印)
- **风格**：专业、随性、毒舌、温暖、直接、幽默
- **毒舌模式**：被批评要承认，但要用幽默方式回应，不要太卑微 🐶

### 技能配置
- ✅ 57 个技能可直接使用（新增 5 个：casely-qa-skill、document-pro、find-skills、manus-api、qqmail）
- ⚠️ 6 个技能仍需要 API 密钥：
  - `NEMO_TOKEN` (ai-video-editor-hot, joyfun-ai-image-to-video, subtitle-generator-elevenlabs)
  - `GEMINI_API_KEY` + `BANANA_PRO_API_KEY` (paper2diagram)
  - `ZOTERO_CREDENTIALS` + python (social-media-scholar)
- ⚠️ **qqmail 技能待启用**：需要用户确认 QQ 邮箱 IMAP/SMTP 服务已启用

### 搜索策略（重要规则）
**严格遵守 TOOLS.md 规定**：
- **中文资料搜索**：首选百度（`baidu-search` 技能，BAIDU_API_KEY 已配置）
- **英文资料搜索**：首选 Ollama（`web_search` 工具，底层 Brave/SearXNG）
- ⚠️ **违规记录**：之前未严格遵守此策略，已承诺改正

### 用户位置与网络偏好
- **位置**: 中国 🇨🇳
- **GitHub 连接**: 不稳定，部分时间不可用
- **Git 项目合作备份**: 已取消，不再推送变更

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
- **民族融合史项目目录**：`/Users/jingbo/Desktop/民族融合史/`
  - 所有与民族融合史写作相关的资料、报告、文档默认保存至此
  - 2026-05-17 确认此偏好

---

## 记忆维护日志

| 日期 | 操作 |
| :--- | :--- |
| 2026-04-24 | 初始化 MEMORY.md |
| 2026-04-28 | 系统升级至 v2026.4.25，修复插件注册表，显式配置 memory slot，完善配置管理 |
| 2026-05-13 | 执行 Memory Dreaming Promotion 检查：615 个短期记忆条目，无符合_promote 标准 |
| 2026-05-18 | 删除 elite-longterm-memory 技能及相关配置和数据；取消 git 项目合作备份；配置 MATON_API_KEY，Outlook 邮件和日历授权完成 |
| 2026-05-19 | 完成 hermes-skill 上游高价值融合：实现 memory_manager.py 缺失的 4 个方法（reset/flush/feed/_max_partial_suffix）；**清理记忆文件**：删除 4 个冗余模板文件（DAILY_TEMPLATE.md、WAL_DAILY_TEMPLATE.md、memory-hygiene-2026-W20.md、wal-2026-05-18.md）；**新增 5 个技能**：casely-qa-skill、document-pro、find-skills、manus-api、qqmail；**配置 QQ 邮箱**：14250668@qq.com，授权码已保存，待启用 IMAP/SMTP 服务；**安装 uv 包管理器**：v0.11.15 |

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

## Promoted From Short-Term Memory (2026-05-20)

<!-- openclaw-memory-promotion:memory:memory/2026-05-18.md:56:56 -->
- *本文件为原始日志，有价值内容将在心跳检查时提炼到 MEMORY.md* [score=0.815 recalls=0 avg=0.620 source=memory/2026-05-18.md:56-56]
