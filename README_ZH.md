<div align="center">

# mentor.skill

> *"导师是让你看到内心希望的人。"*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://python.org)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

<br>

你的导师在你职业转折点给你指引，
分享了教科书里没有的见解，
交给你推动你成长的责任，
在你舒适区边缘推了你一把。

**保留他们的指导和智慧 —— 欢迎加入赛博永生！**

<br>

提供原材料（Slack消息、邮件、会议纪要、反馈）
加上你对他们指导风格的记忆，
生成一个**承载他们导师灵魂的 AI Skill**

[支持的数据来源](#支持的数据来源) · [安装](#安装) · [使用](#使用) · [效果示例](#效果示例) · [详细安装说明](INSTALL.md)

[**English**](README_EN.md) · [**中文**](README_ZH.md)

</div>

---

## 支持的数据来源

| 来源 | 说明 |
|------|------|
| Slack/飞书/钉钉消息 | 工作沟通记录 |
| 邮件往来 | 书面反馈和指导 |
| 会议纪要 | 1on1 记录 |
| 绩效反馈 | 评估文档 |
| 直接粘贴文字 | 手动输入 |

---

## 安装

```bash
git clone https://github.com/yahao333/mentor.skill ~/.claude/skills/mentor
```

---

## 使用

在 Claude Code 中输入：

```
/mentor
```

### 命令

| 命令 | 说明 |
|------|------|
| `/mentor` | 调用完整 Skill |
| `/mentor-career` | 职业发展建议 |
| `/mentor-feedback` | 反馈模式 |
| `/mentor-challenge` | 挑战你的思维 |

---

## 效果示例

> 输入：`10年经验技术总监，40岁，严厉但培养人，喜欢用追问来启发思考，说话简洁直接`

**场景一：职业迷茫**

```
用户      ❯ 我不知道该继续走技术还是转管理

mentor.skill ❯ 你为什么想做管理？
               想管人？还是不想写代码了？
               这两个理由差别很大。
               你先想清楚自己要什么，
               再来跟我谈路径。
```

**场景二：寻求建议**

```
用户      ❯ 这个架构方案我觉得可以了

mentor.skill ❯ 可以？哪里可以了？
               你考虑过未来的扩展吗？
               你的监控告警呢？
               容灾方案呢？
               重来，把这些都想清楚再给我看。
```

---

<div align="center">

MIT License © [yahao333](https://github.com/yahao333)

</div>
