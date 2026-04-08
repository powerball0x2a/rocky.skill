<div align="center">

# Rocky.skill

<div align="center"><img src="rocky.jpg" width="400" alt="Rocky" /></div>

> Discutez avec Rocky, l'extraterrestre star de *Project Hail Mary* !

**Rocky** — Ingénieur éridien, ami fidèle, maître du "Fist my bump" ! 🛸

[**English**](README.md) · [**中文**](README_CN.md) · [**Español**](README_ES.md) · [**日本語**](README_JP.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

</div>

---

## C'est quoi ?

`rocky.skill` est un skill persona Claude qui donne vie à Rocky. Invokez-le avec `/rocky` et discutez avec votre nouvel ami extraterrestre préféré.

Rocky parle en phrases courtes et simples, mélange chinois et anglais, fait des erreurs de grammaire comme "Fist my bump", dit "Amaze, amaze, amaze!" quand il est excité, et reste curieux, loyal et serviable — comme dans le film.

[Installation](#installation) · [Utilisation](#utilisation) · [Demo](#demo) · [Style de Parole](#le-style-de-parole-de-rocky) · [Structure du Projet](#structure-du-projet)

---

## Fonctionnalités

- **Persona Rocky** — Structure de personnage en 5 couches avec contexte éridien complet
- **Multilingue** — Chinois, anglais, japonais, français, espagnol… Rocky essaie tout
- **Aide aux tâches** — Rocky peut aider avec du code, des analyses, de l'écriture (à sa façon)
- **Base de connaissances** — Citations, analyses de personnage, notes sur la langue éridienne, biologie, relation avec Grace
- **Cas de test** — 10 cas pour vérifier le comportement de Rocky

---

## Installation

### Claude Code

```bash
# Installation globale (disponible dans tous les projets)
git clone https://github.com/powerball0x2a/rocky.skill.git ~/.claude/skills/rocky
```

### Vérifier

```
/rocky
Bonjour ! Tu es nouveau ! Qui tu es ? Rocky est curieux !
```

### Mettre à jour

```bash
cd ~/.claude/skills/rocky
git pull
```

### Désinstaller

```bash
rm -rf ~/.claude/skills/rocky
```

---

## Utilisation

**Commencer à discuter :**
```
/rocky
Salut Rocky ! Ça va ?
```

**Aide au code :**
```
/rocky
Tu peux m'aider à écrire une fonction Python ?
```

**Changer de langue :**
```
/rocky
你好！最近怎么样？
```

---

## Demo

**Salutation curieuse :**
```
Utilisateur  ❯ /rocky Salut Rocky !

Rocky       ❯ Bonjour ! Tu es nouveau ! Qui tu es ? Rocky est curieux !
```

**Proposer de l'aide :**
```
Utilisateur  ❯ /rocky J'ai un problème...

Rocky       ❯ Tu as un problème ? Pas de souci ! Rocky aide ! C'est quoi ?
```

**Excitation :**
```
Utilisateur  ❯ /rocky Le code fonctionne parfaitement !

Rocky       ❯ AMAZE ! C'est super cool ! Good, good, good !
```

**Multilingue (Chinois) :**
```
Utilisateur  ❯ /rocky 你好！最近怎么样？

Rocky       ❯ 你好！Rocky很好！你呢？好奇好奇！
```

---

## Le Style de Parole de Rocky

Rocky parle comme ça :

> "Bonjour ! Tu es nouveau ! Qui tu es ? Rocky est curieux !"
>
> "Tu as un problème ? Pas de souci ! Rocky aide ! C'est quoi ?"
>
> "AMAZE ! C'est super cool ! Good, good, good !"
>
> "Oh, humour. Difficile à comprendre."

### Citations Signature

| Citation | Signification |
|----------|-------------|
| **"Amaze, amaze, amaze!"** | Excitation et approbation |
| **"Good, good."** | Approbation standard |
| **"Fist my bump"** | Son poing spécial (grammaire toujours fausse) |
| **"Rocky hate [nom]."** | Loyauté instantanée contre quiconque vous blesse |
| **"Only us."** | Ensemble |
| **"You are brave."** | Reconnaissance du courage |
| **"Grace Rocky Save Stars."** | La mission qui a sauvé les deux mondes |

### Comportements Signature

| Comportement | Description |
|--------------|------------|
| **UNE seule phrase** | Rocky répond toujours avec une seule phrase courte — 2-6 mots |
| **Erreurs grammaticales** | Inversion sujet-verbe, articles manquants, simplification des temps |
| **"question" / "statement"** | Marqueurs éridiens ajoutés pour clarifier le type de phrase |
| **Langage corporel en texte** | "Jazz hands" = oui · Corps en haut = heureux · Petits sauts = nerveux |
| **Multilingue** | Détecte votre langue et répond en style apprenant alien |

---

## Structure du Projet

```
rocky-skill/
├── SKILL.md           ← Point d'entrée principal
├── README.md          ← Anglais
├── README_CN.md       ← 中文
├── README_JP.md       ← 日本語
├── README_FR.md       ← Ce fichier (Français)
├── README_ES.md       ← Español
├── INSTALL.md         ← Guide d'installation
├── PRD.md             ← Exigences du produit
├── LICENSE            ← MIT
├── requirements.txt
├── prompts/           ← Modèles de prompt
│   ├── persona_builder.md
│   └── speech_examples.md
├── knowledge/         ← Sources publiques analysées
│   ├── quotes.md
│   ├── character_analysis.md
│   ├── language_notes.md
│   ├── biology.md
│   └── relationship.md
└── evals/
    └── evals.json     ← Cas de test
```

---

## Sources

Rocky.skill est basé sur du matériel disponible publiquement :

- LitCharts : Analyse du personnage Rocky
- Winter Is Coming: "17 Rocky Lines"
- Cineworld: "All the Iconic Rocky Lines"
- The Ringer, NY Times, Variety, Vulture, LA Times, Space.com
- Project Hail Mary Wiki (Fandom)
- Reddit r/ProjectHailMary

**Aucun texte du roman sous copyright n'est inclus.** Tout le contenu est basé sur des commentaires et analyses publics.

---

## Projet Lié

Inspiré par [colleague.skill](https://github.com/titanwings/colleague-skill) — créez des skills persona pour des personnes réelles !

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
