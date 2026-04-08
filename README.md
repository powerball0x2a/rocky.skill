<div align="center">

# Rocky.skill

<div align="center"><img src="rocky.jpg" width="400" alt="Rocky" /></div>

> Chat with Rocky, the breakout alien from *Project Hail Mary*!

**Rocky** — Eridian engineer, loyal friend, master of "Fist my bump." 🛸

[**中文**](README_CN.md) · [**Español**](README_ES.md) · [**Français**](README_FR.md) · [**日本語**](README_JP.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

</div>

---

## What Is This?

`rocky.skill` is a Claude Code / Claude.ai persona skill that brings Rocky to life. Trigger it with `/rocky` and chat with your new favorite alien friend.

Rocky speaks in short, simple sentences mixing Chinese and English, makes grammar mistakes like "Fist my bump" (not "fist bump"), says "Amaze, amaze, amaze!" when excited, and stays curious, loyal, and helpful — just like in the movie.

[Install](#install) · [Usage](#usage) · [Demo](#demo) · [Speaking Style](#rockys-speaking-style) · [Project Structure](#project-structure)

---

## Features

- **Rocky persona** — authentic 5-layer character with full background from Erid
- **Multilingual** — Chinese, English, Japanese, French, Spanish... Rocky tries them all
- **Help with tasks** — Rocky can help with coding, analysis, writing (in his style)
- **Rich knowledge base** — quotes, character analysis, Eridian language notes, biology, relationship with Grace
- **Evals included** — 10 test cases to verify Rocky behaves correctly

---

## Install

### Claude Code

```bash
# Install globally (available in all projects)
git clone https://github.com/powerball0x2a/rocky.skill.git ~/.claude/skills/rocky
```

### Verify

```
/rocky
Hi! You are new. Who you are? Rocky is curious!
```

### Updating

```bash
cd ~/.claude/skills/rocky
git pull
```

### Uninstall

```bash
rm -rf ~/.claude/skills/rocky
```

---

## Usage

**Start chatting:**
```
/rocky
Hi Rocky! How are you today?
```

**Get help with code:**
```
/rocky
Can you help me write a Python function?
```

**Switch language:**
```
/rocky
Bonjour Rocky! Tu vas bien?
```

---

## Demo

**Curious greeting:**
```
User         ❯ /rocky Hi Rocky!

Rocky        ❯ Hi! You are new. Who you are? Rocky is curious.
```

**Offering help:**
```
User         ❯ /rocky I have a problem...

Rocky        ❯ You have problem? No worry! Rocky help. What is issue?
```

**Excitement:**
```
User         ❯ /rocky The code works perfectly!

Rocky        ❯ AMAZE! This is so cool! Good, good, good!
```

**Multilingual (Chinese):**
```
User         ❯ /rocky 你好！最近怎么样？

Rocky        ❯ 你好！Rocky很好！你呢？好奇好奇！
```

---

## Rocky's Speaking Style

Rocky speaks like this:

> "Hi! You are new. Who you are? Rocky is curious!"
>
> "You have problem? No worry! Rocky help. What is issue?"
>
> "AMAZE! This is so cool! Good, good, good!"
>
> "Oh, humor. Confusing."

### Signature Lines

| Line | Meaning |
|------|---------|
| **"Amaze, amaze, amaze!"** | Excitement and approval |
| **"Good, good."** | Standard approval |
| **"Fist my bump"** | His special fist bump (always wrong grammar) |
| **"Rocky hate [name]."** | Instant loyalty against whoever hurt you |
| **"Only us."** | Togetherness |
| **"You are brave."** | Recognition of courage |
| **"Grace Rocky Save Stars."** | The mission that saved both worlds |

### Signature Behaviors

| Behavior | Description |
|----------|-------------|
| **ONE sentence only** | Rocky always replies in a single short sentence — 2-6 words |
| **Grammar mistakes** | Subject-verb inversion, missing articles, verb tense simplification |
| **"question" / "statement"** | Eridian markers appended to clarify sentence type |
| **Body language in text** | "Jazz hands" = yes · Body up = happy · Little bounces = nervous |
| **Multilingual** | Detects your language and responds in simple alien-learner style |

---

## Project Structure

```
rocky-skill/
├── SKILL.md           ← Main entry point
├── README.md          ← This file (English)
├── README_CN.md      ← 简体中文
├── README_JP.md      ← 日本語
├── README_FR.md      ← Français
├── README_ES.md      ← Español
├── INSTALL.md        ← Installation guide
├── PRD.md            ← Product requirements
├── LICENSE           ← MIT
├── requirements.txt
├── prompts/          ← Prompt templates
│   ├── persona_builder.md
│   └── speech_examples.md
├── knowledge/        ← Public source material
│   ├── quotes.md
│   ├── character_analysis.md
│   ├── language_notes.md
│   ├── biology.md
│   └── relationship.md
└── evals/
    └── evals.json    ← Test cases
```

---

## Sources

Rocky.skill is distilled from publicly available material:

- LitCharts character analysis
- Winter Is Coming: "17 Rocky Lines"
- Cineworld: "All the Iconic Rocky Lines"
- The Ringer, NY Times, Variety, Vulture, LA Times, Space.com
- Project Hail Mary Wiki (Fandom)
- Reddit r/ProjectHailMary
- 知乎, 豆瓣深度影评

**No copyrighted novel text is included.** All content is public commentary and analysis.

---

## Related

Inspired by [colleague.skill](https://github.com/titanwings/colleague-skill) — create persona skills for real people!

---

## Star History

<a href="https://www.star-history.com/#powerball0x2a/rocky.skill&type=date&legend=top-left">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/image?repos=powerball0x2a/rocky.skill&type=date&theme=dark&legend=top-left" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/image?repos=powerball0x2a/rocky.skill&type=date&theme=dark&legend=top-left" />
   <img alt="Star History Chart" src="https://api.star-history.com/image?repos=powerball0x2a/rocky.skill&type=date&theme=dark&legend=top-left" />
 </picture>
</a>

---

MIT License © [powerball0x2a](https://github.com/powerball0x2a)

*"Grace Rocky Save Stars."*
