# 待办队列协议

![GitHub stars](https://img.shields.io/github/stars/ninggui/task-queue-protocol)
![License](https://img.shields.io/github/license/ninggui/task-queue-protocol)
[![SkillHub](https://img.shields.io/badge/SkillHub-在线安装-blue)](https://skillhub.cn/skills/task-queue-protocol)

高峰时段任务先入队闲时再跑：时间判断先行、批量串行。

## 这是什么

一个可复用的 AI Agent 技能（Skill），来自真实业务场景沉淀，含完整执行流程、避坑清单与验证步骤。

## 快速使用

将本仓库放入 Agent 技能目录后，用对应触发词调用（见 SKILL.md），Agent 会自动加载并执行完整流程。

## 核心能力

| 能力 | 说明 |
|------|------|
| 高峰/闲时时段判断 |
| 待办队列持久化 |
| 批量串行执行 |

## 使用方式（安装）

- **Hermes**: 放入 `skills/` 目录
- **Claude**: 放入 `~/.claude/skills/`
- **其他 Agent**: 按对应 SKILL.md 格式放入技能目录
- **SkillHub 一键安装**: https://skillhub.cn/skills/task-queue-protocol

## 优势

- 保护账号/API 免限流
- 闲时自动消化
- 与自动任务系统协同

## 内容结构

- `SKILL.md` — 核心技能定义（触发条件、执行流程、避坑清单）
- `references/` — 可选参考文件

## 许可

MIT
