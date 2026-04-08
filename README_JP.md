<div align="center">

# Rocky.skill

<div align="center"><img src="rocky.jpg" width="400" alt="Rocky" /></div>

> Project Hail Mary の人気宇宙人Rockyとチャットしよう！

**Rocky** — エリディアンエンジニア、忠诚な友達、「Fist my bump」のマスター！🛸

[**English**](README.md) · [**中文**](README_CN.md) · [**Español**](README_ES.md) · [**Français**](README_FR.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

</div>

---

## これは何？

`rocky.skill` はRockyを再現するClaude Code / Claude.ai personaスキルです。`/rocky` で起動すると、大好きな宇宙人の友達とチャットできます。

Rockyは短くシンプルな文で話し中国語と英語を組み合わせ、文法錯誤（比如「Fist my bump」）、興奮すると「Amaze, amaze, amaze!」と言い、いつも好奇心が強く、忠诚で、助けるのが好き——映画と同じです。

[インストール](#インストール) · [使い方](#使い方) · [デモ](#デモ) · [話し方](#rocky-の話し方) · [プロジェクト構造](#プロジェクト構造)

---

## 機能

- **Rocky 人格** — 5層キャラクター構造、完整的Erid背景
- **多言語サポート** — 中国語、英語、日本語、フランス語、スペイン語…Rockyは全部試す
- **タスク支援** — Rockyはコード書き、分析、文章作成を手伝わる（彼のスタイルで）
- **知識ベース** — 名台詞、キャラクター分析、Eridian言語メモ、生物学背景 Graceとの絆
- **テストケース** — Rockyの行動を検証する10のテスト

---

## インストール

### Claude Code

```bash
# グローバルインストール（全てのプロジェクトで利用可能）
git clone https://github.com/powerball0x2a/rocky.skill.git ~/.claude/skills/rocky
```

### 確認

```
/rocky
你好！你是新来的！你叫什么名字？Rocky 很感兴趣！
```

### アップデート

```bash
cd ~/.claude/skills/rocky
git pull
```

### アンインストール

```bash
rm -rf ~/.claude/skills/rocky
```

---

## 使い方

**チャット開始：**
```
/rocky
Rocky、元気？今天有何新鮮？
```

**コードを書くのを手伝う：**
```
/rocky
Pythonの関数を手伝ってくれない？
```

**言語を切り替える：**
```
/rocky
Bonjour Rocky! Tu vas bien?
```

---

## デモ

**好奇心の挨拶：**
```
ユーザー   ❯ /rocky 你好 Rocky！

Rocky      ❯ 你好！你是新来的！你叫什么名字？Rocky 很感兴趣！
```

** помощь を申し出る：**
```
ユーザー   ❯ /rocky 問題がある...

Rocky      ❯ 問題がある？大丈夫！Rocky が手伝う！何の問題？
```

**興奮：**
```
ユーザー   ❯ /rocky コードが完璧に動いた！

Rocky      ❯ AMAZE！这是太棒了！Good, good, good!
```

**多言語（法语）：**
```
ユーザー   ❯ /rocky Salut Rocky! Ça va?

Rocky      ❯ Bonjour! Tu es nouveau! Rocky est curieux!
```

---

## Rocky の話し方

Rockyはこう言います：

> "你好！你是新来的！你叫什么名字？Rocky 很感兴趣！"
>
> "問題がある？大丈夫！Rocky が手伝う！何の問題？"
>
> "AMAZE！这是太棒了！Good, good, good!"
>
> "Oh、ユーモア。わからない。"

### シグネチャーライン

| セリフ | 意味 |
|--------|------|
| **"Amaze, amaze, amaze!"** | 興奮と认可 |
| **"Good, good."** | 標準的な认可 |
| **"Fist my bump"** | 彼の专属ファストバンプ（文法いつも間違い） |
| **"Rocky hate [名前]."** | 即座に味方の立場を取る |
| **"Only us."** | 一緒にいる |
| **"You are brave."** | 勇敢さを認め |
| **"Grace Rocky Save Stars."** | 両世界救了使命 |

### シグネチャー行動

| 行動 | 説明 |
|------|------|
| **一句话だけ** | Rockyは常に一つの短い文で返信 — 2-6語 |
| **文法錯誤** | 主語-動詞の倒置冠詞欠落 時制単純化 |
| **"question" / "statement"** | 文の種類を明確にするEridian マーカー |
| **テキスト内ボディーランゲージ** | "Jazz hands" = はい · 体上 = 幸せ · 小さな跳躍 = 緊張 |
| **多言語** | ユーザーの言語を検出し宇宙人学習者風に返信 |

---

## プロジェクト構造

```
rocky-skill/
├── SKILL.md           ← メインエントリ
├── README.md          ← 英語
├── README_CN.md       ← 中文
├── README_JP.md       ← このファイル（日本語）
├── README_FR.md       ← Français
├── README_ES.md       ← Español
├── INSTALL.md         ← インストールガイド
├── PRD.md             ← 製品要件
├── LICENSE            ← MIT
├── requirements.txt
├── prompts/           ← プロンプトテンプレート
│   ├── persona_builder.md
│   └── speech_examples.md
├── knowledge/         ← 公開资料的まとめ
│   ├── quotes.md
│   ├── character_analysis.md
│   ├── language_notes.md
│   ├── biology.md
│   └── relationship.md
└── evals/
    └── evals.json     ← テストケース
```

---

## 資料來源

Rocky.skillは公開資料から生み出されています：

- LitCharts キャラクター分析
- Winter Is Coming: "17 Rocky Lines"
- Cineworld: "All the Iconic Rocky Lines"
- The Ringer, NY Times, Variety, Vulture, LA Times, Space.com
- Project Hail Mary Wiki (Fandom)
- Reddit r/ProjectHailMary
- 中国語・日本語レビュー・分析

**的小説原文は含みません。** 全て公開コメントと分析です。

---

## 関連プロジェクト

着想源 [colleague.skill](https://github.com/titanwings/colleague-skill) — 実在の人物のpersonaスキルを作成しよう！

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
