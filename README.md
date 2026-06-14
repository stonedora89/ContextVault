# ContextVault
阅读驱动的场景英语学习系统

# ContextVault

> Learn from Reading, Remember by Context

Version: MVP 1.0

---

# 产品定位

ContextVault 不是背单词软件。

也不是传统英语学习软件。

它是一个：

**阅读驱动（Reading Driven）**
**场景驱动（Scenario Driven）**
**AI辅助记忆（AI Assisted Learning）**

的个人英语知识库。

核心理念：

```text
阅读
↓
收藏
↓
理解场景
↓
AI扩展
↓
长期记忆
```

而不是：

```text
单词
↓
中文
↓
死记硬背
```

---

# 解决的问题

用户在阅读：

* PDF
* 网页
* 技术文档
* 标准
* 英文书籍
* Markdown

时经常遇到：

* 好的句子
* 专业表达
* 高频术语
* 面试表达
* 工作场景表达

但：

* 收藏后不会复习
* 只记单词不会使用
* 无法形成长期记忆

ContextVault解决：

```text
记住句子
记住场景
顺便记住单词
```

---

# 用户群体

## 技术人员

* IEC62443
* CISSP
* ISO27001
* IT
* OT
* Security

---

## 开发者

* Swift
* AI
* Python
* Cloud

---

## HR

* Interview
* Recruitment
* Performance

---

## 普通英语学习者

* Daily English
* Business English

---

# 核心原则

## 场景优先

不是：

```text
Word
```

而是：

```text
Scenario
↓
Sentence
↓
Phrase
↓
Word
```

---

## 句子优先

系统核心对象：

```text
Sentence
```

不是：

```text
Word
```

---

## 学习优先

收藏只是开始。

学习才是最终目的。

---

# 信息架构

## Domain（领域）

例如：

```text
IEC62443
ISO27001
CISSP
AI开发
Swift开发
HR
日常英语
```

---

## Scenario（场景）

IEC62443

```text
Zone & Conduit
Risk Assessment
Patch Management
Access Control
Incident Response
```

---

AI

```text
Prompt Engineering
RAG
Agent
Embedding
MCP
```

---

HR

```text
Interview
Recruitment
Performance
```

---

## Sentence

核心对象

```text
The asset owner shall establish
zones and conduits.
```

---

## Word

附属对象

```text
conduit
zone
asset owner
```

---

# 收藏流程

用户：

```text
阅读网页
阅读PDF
阅读文档
```

选中：

```text
单词
短语
句子
```

快捷键：

```text
⌘ + Shift + S
```

弹窗：

```text
Save to ContextVault

领域：
IEC62443

场景：
Zone & Conduit

收藏原因：
□ 考试重点
□ 专业术语
□ 工作常用
□ 写得很好

Save
```

---

# 数据模型

## Sentence

```swift
Sentence

id

originalText

translation

source

sourceURL

domain

scenario

topic

whySaved

masteryLevel

difficulty

createdAt

updatedAt
```

---

## Word

```swift
Word

id

word

phonetic

meaning

domain

linkedSentences
```

---

# AI能力

## AI解释

解释：

```text
为什么重要
```

例如：

```text
The asset owner shall establish
zones and conduits.
```

AI：

```text
这是IEC62443网络分区设计中的核心要求。
```

---

## AI扩展表达

自动生成：

```text
类似表达
```

例如：

```text
Security zones shall be defined.

A secure conduit must be established.

Communication between zones shall be controlled.
```

---

## AI应用场景

自动生成：

```text
真实工作中如何使用
```

---

## AI生成练习

### 填空

```text
The asset owner shall establish
zones and ______.
```

---

### 中译英

```text
资产所有者应建立区域和通信通道。
```

---

### 场景题

```text
Conduit 通常与哪个概念一起出现？

Zone
Firewall
Patch
```

---

# 学习系统

## 掌握度

```text
0 不会

1 模糊

2 认识

3 基本掌握

4 已掌握

5 归档
```

---

## 复习策略

不会：

```text
每天
```

---

模糊：

```text
2天
```

---

认识：

```text
7天
```

---

掌握：

```text
30天
```

---

归档：

```text
仅搜索可见
```

---

# UI设计

## 左侧导航

```text
📚 今日学习

🗂 场景库

📖 收藏库

📕 单词本

🔍 搜索

📊 统计

⚙ 设置
```

---

## 场景库

```text
IEC62443
│
├─ Zone & Conduit
├─ Risk Assessment
├─ Patch Management
├─ Access Control

AI开发
│
├─ RAG
├─ Agent
├─ Prompt

HR
│
├─ Interview
├─ Recruitment
```

---

## 中间区域

显示：

```text
句子列表
```

例如：

```text
The asset owner shall establish
zones and conduits.

Risk assessment should be
performed regularly.
```

---

## 右侧区域

显示：

```text
使用场景

AI解释

类似表达

涉及词汇

我的笔记
```

---

## 底部学习栏

```text
😵 不会

😐 模糊

🙂 认识

😎 掌握

⏭ 跳过
```

---

# MVP范围

必须实现

```text
✓ 收藏句子

✓ 收藏单词

✓ 场景分类

✓ 搜索

✓ AI解释

✓ AI扩展表达

✓ 掌握度系统

✓ 今日学习

✓ 复习计划
```

---

暂不实现

```text
✗ iPhone

✗ 云同步

✗ 多用户协作

✗ 社区

✗ 浏览器插件
```

---

# 产品核心价值

ContextVault 不帮助用户背单词。

ContextVault 帮助用户：

```text
从真实阅读中学习

从场景中理解

从句子中记忆

从AI中扩展

最终形成长期记忆
```
