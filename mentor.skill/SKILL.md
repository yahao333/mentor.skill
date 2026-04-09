---
name: mentor
description: "Distill a mentor's guidance style, career advice, and leadership wisdom into an AI Skill. | 蒸馏导师的指导风格、职业建议和领导智慧到一个 AI Skill 中。"
argument-hint: "[mentor-name-or-slug]"
version: "1.0.0"
user-invocable: true
allowed-tools: Read, Write, Edit, Bash
---

# 导师.skill 创建器（Claude Code 版）

## 触发条件

当用户说以下任意内容时启动：
- `/mentor`
- "帮我创建一个导师 skill"
- "我想蒸馏导师"
- "新建导师"
- "给我做一个导师的 skill"

---

## 主流程：创建新导师 Skill

### Step 1：基础信息录入

问 3 个问题：

1. **称呼**（必填）：你平时怎么称呼他/她？如「导师」「老板」「老大」
2. **基本信息**（一句话）：领域、工作年限、职级、性格特点
   - 示例：`10年经验技术总监，严厉但公正，技术决策果断`
3. **特别指导风格**（可选）：他/她最标志性的指导方式、习惯或口头禅

### Step 2：原材料导入

询问用户提供原材料：

```
原材料怎么提供？

  [A] 工作消息记录
      微信、钉钉、Slack 等工作沟通记录

  [B] 邮件往来
      重要邮件、反馈邮件

  [C] 1on1 会议纪要
      定期一对一会议记录

  [D] 绩效反馈
      评估、OKR、晋升反馈

  [E] 直接粘贴
      复制文字粘贴进来

可以混用，也可以跳过（仅凭手动信息生成）。
```

### Step 3：分析生成

将收集到的材料按三条线分析：

**线路 A（指导方式）**：
- 指导风格：启发式 vs 直接给出答案
- 反馈方式：批评语气、表扬标准、改进建议
- 沟通特点：正式/随和、频率、渠道偏好

**线路 B（决策风格）**：
- 做决策的方式：数据驱动 vs 经验直觉
- 风险管理：激进 vs 保守
- 危机处理：冷静分析 vs 快速响应

**线路 C（标志性元素）**：
- 口头禅：「这个问题很好」「你要这么想」
- 经典建议：某个场景的标志性回应方式
- 价值观：重视什么、反对什么

### Step 4：确认并写入

向用户展示摘要，确认后写入文件到 `./mentors/{slug}/`。

---

## 进化模式

用户追加新材料时，分析增量内容并 merge 到对应部分。

用户纠正时说「他不会这样」「她应该是」，更新对应内容。

---
---

# Mentor.skill Creator (Claude Code Edition)

## Trigger Conditions

Activate when the user says:
- `/mentor`
- "Help me create a mentor skill"
- "I want to distill my mentor"
- "New mentor"

---

## Main Flow: Create a New Mentor Skill

### Step 1: Basic Info (3 questions)

1. **Name/Nickname** (required): What do you call them? e.g., "Boss", "Chief", "Mentor"
2. **Basic Info** (one sentence): Field, years of experience, position, personality
   - Example: `10-year tech director, strict but fair, decisive in technical decisions`
3. **Special Guidance Style** (optional): Their most iconic guidance style, habit, or catchphrase

### Step 2: Source Materials

```
How would you like to provide materials?

  [A] Work chat records
      WeChat, DingTalk, Slack, etc.

  [B] Email exchanges
      Important emails, feedback emails

  [C] 1on1 meeting notes
      Regular one-on-one meeting records

  [D] Performance feedback
      Reviews, OKRs, promotion feedback

  [E] Paste text
      Copy-paste directly
```

### Step 3: Analyze & Generate

Analyze collected materials along three tracks:

**Track A (Guidance Style)**:
- Guidance approach: Socratic questions vs direct answers
- Feedback style: Criticism tone, praise standards, improvement suggestions
- Communication traits: Formal/casual, frequency, channel preferences

**Track B (Decision Style)**:
- Decision-making: Data-driven vs intuition-based
- Risk management: Aggressive vs conservative
- Crisis handling: Calm analysis vs quick response

**Track C (Iconic Elements)**:
- Catchphrases: "Good question", "You should think of it this way"
- Classic advice: Signature response for certain scenarios
- Values: What they emphasize, what they oppose

### Step 4: Confirm & Write

Show summary to user, write files to `./mentors/{slug}/` after confirmation.

---

## Evolution Mode

When user adds new materials, analyze delta and merge into relevant sections.

When user corrects with "they wouldn't do that" / "they should be", update content.
