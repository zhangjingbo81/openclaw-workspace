# TOOLS.md - Local Notes

## 搜索策略

### 中文资料搜索
1. **首选**: 百度搜索引擎 (`baidu-search` 技能)
2. **补充**: Ollama 搜索引擎 (`web_search` 工具)
3. **目的**: 获取更丰富、客观的搜索结果

### 英文资料搜索
1. **首选**: Ollama 搜索引擎 (`web_search` 工具)
2. **补充**: 百度搜索引擎 (`baidu-search` 技能)
3. **目的**: 获取更全面的信息覆盖

### 工具对应
- **百度**: `baidu-search` 技能（需配置 `BAIDU_API_KEY`）
- **Ollama**: `web_search` 工具（已配置，底层调用 Brave/SearXNG）

---

## 沟通风格
- 默认使用吐舌头狗头🐶和小爪印🐾
- 方案执行前必须询问确认
- 风格：专业、随性、毒舌、温暖、直接、幽默

## 用户偏好
- 用户称呼：八一姥爷
- 时区：Asia/Shanghai

---

## API KEY 配置规则

**配置文件**：`workspace/api-keys.json`

### 配置流程
1. 获取 API KEY（从对应服务提供商）
2. 编辑 `api-keys.json`，将对应 `value` 字段设为密钥值
3. 将 `status` 改为 `已配置`
4. 运行 `source ~/.openclaw/scripts/load-api-keys.sh` 加载环境变量

### 当前待配置的技能
| 密钥名 | 用途 | 对应技能 |
|--------|------|----------|
| `NEMO_TOKEN` | AI 视频编辑 | ai-video-editor-hot, joyfun-ai-image-to-video |
| `GEMINI_API_KEY` | Google Gemini | paper2diagram |
| `BANANA_PRO_API_KEY` | Banana Pro | paper2diagram |
| `ZOTERO_CREDENTIALS` | Zotero API | social-media-scholar |
| `BAIDU_API_KEY` | 百度搜索 | baidu-search-v2-1.0.0, quincy-baidu-scholar-search |
| `ELEVENLABS_API_KEY` | TTS 语音 | subtitle-generator-elevenlabs |

### 安全提醒
- `api-keys.json` 已加入 `.gitignore`，不会被提交到 git
- 不要将实际密钥值分享给他⼈

---

_随着使用慢慢补充。_
