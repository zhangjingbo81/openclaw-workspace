# QQ 邮箱配置记录

## 配置信息
- **邮箱地址**: 14250668@qq.com
- **授权码**: 已配置（197981106）
- **配置时间**: 2026-05-19

## 问题记录

### 2026-05-19 10:40 - 登录失败
**错误信息**: `Login fail. Account is abnormal, service is not open, password is incorrect, login frequency limited, or system is busy`

**可能原因**:
1. QQ 邮箱的 IMAP/SMTP 服务未启用
2. 授权码不正确或已过期
3. 账号有安全风险被限制

**解决步骤**:
1. 登录 mail.qq.com
2. 进入「设置」→「账户」
3. 确保「IMAP/SMTP 服务」已启用
4. 重新生成授权码（如果旧授权码失效）
5. 确保使用授权码而非 QQ 密码

**状态**: ⚠️ 待解决 - 需要用户确认 IMAP/SMTP 服务是否已启用

## qqmail 技能配置
- 路径: `~/.openclaw/workspace/skills/qqmail-1-0-0-1.0.0/`
- 环境变量: QQMAIL_USER, QQMAIL_AUTH_CODE
- SSL 证书问题已修复（使用 certifi）
