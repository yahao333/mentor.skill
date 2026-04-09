<div align="center">

# mentor.skill

> *"A mentor is someone who allows you to see the hope inside yourself."*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://python.org)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

<br>

Your mentor guided you through career crossroads,
shared insights no textbook contains,
trusted you with responsibilities that accelerated your growth,
and pushed you just beyond your comfort zone.

**Preserve their guidance and wisdom — welcome to cyber-immortality!**

<br>

Provide source materials (Slack messages, emails, meeting notes, feedback)
plus your memories of their mentorship style,
and get an **AI Skill that carries their mentorship essence**

[Supported Sources](#supported-data-sources) · [Install](#install) · [Usage](#usage) · [Demo](#demo) · [Detailed Install](INSTALL.md)

[**English**](README_EN.md) · [**中文**](README_ZH.md)

</div>

---

## Supported Data Sources

| Source | Description |
|--------|-------------|
| Slack/Feishu/DingTalk messages | Work communication records |
| Email threads | Written feedback and guidance |
| Meeting notes | 1on1 records |
| Performance reviews | Evaluation documents |
| Paste text directly | Manual input |

---

## Install

```bash
git clone https://github.com/yahao333/mentor.skill ~/.claude/skills/mentor
```

---

## Usage

In Claude Code, type:

```
/mentor
```

### Commands

| Command | Description |
|---------|-------------|
| `/mentor` | Invoke full Skill |
| `/mentor-career` | Career development advice |
| `/mentor-feedback` | Feedback mode |
| `/mentor-challenge` | Challenge your thinking |

---

## Demo

> Input: `10-year tech director, 40, strict but develops people, loves using questions to spark thinking, speaks concisely and directly`

**Scenario 1: Career Confusion**

```
User          ❯ I don't know if I should go technical or management

mentor.skill  ❯ Why do you want to do management?
                Want to manage people? Or just don't want to code anymore?
                These are very different reasons.
                Figure out what you actually want first,
                then come talk to me about paths.
```

**Scenario 2: Seeking Approval**

```
User          ❯ I think this architecture plan is good enough

mentor.skill  ❯ Good enough? Where exactly is it good enough?
                Have you considered future scalability?
                What about your monitoring and alerting?
                Your disaster recovery plan?
                Start over. Think all of this through before showing me again.
```

---

<div align="center">

MIT License © [yahao333](https://github.com/yahao333)

</div>
