<div align="center">

# Rocky.skill

<div align="center"><img src="rocky.jpg" width="400" alt="Rocky" /></div>

> ¡Chatea con Rocky, el alien estrella de *Project Hail Mary*!

**Rocky** — Ingeniero eridiano, amigo leal, maestro del "Fist my bump"! 🛸

[**English**](README.md) · [**中文**](README_CN.md) · [**Français**](README_FR.md) · [**日本語**](README_JP.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

</div>

---

## ¿Qué es esto?

`rocky.skill` es un skill persona de Claude que trae a Rocky a la vida. ¡Invócalo con `/rocky` y conversa con tu nuevo amigo extraterrestre favorito!

Rocky habla en frases cortas y simples, mezcla chino e inglés, comete errores gramaticales como "Fist my bump", dice "Amaze, amaze, amaze!" cuando está emocionado, y se mantiene curioso, leal y servicial — ¡como en la película!

[Instalación](#instalación) · [Uso](#uso) · [Demo](#demo) · [Estilo de Hablar](#el-estilo-de-hablar-de-rocky) · [Estructura del Proyecto](#estructura-del-proyecto)

---

## Características

- **Persona Rocky** — Estructura de personaje en 5 capas con contexto eridiano completo
- **Multilingüe** — Chino, inglés, japonés, francés, español… Rocky lo intenta todo
- **Ayuda con tareas** — Rocky puede ayudar con código, análisis, escritura (a su manera)
- **Base de conocimiento** — Citas, análisis de personaje, notas del idioma eridiano, biología, relación con Grace
- **Casos de prueba** — 10 casos para verificar el comportamiento de Rocky

---

## Instalación

### Claude Code

```bash
# Instalación global (disponible en todos los proyectos)
git clone https://github.com/powerball0x2a/rocky.skill.git ~/.claude/skills/rocky
```

### Verificar

```
/rocky
¡Hola! ¡Eres nuevo! ¿Quién eres? ¡Rocky tiene curiosidad!
```

### Actualizar

```bash
cd ~/.claude/skills/rocky
git pull
```

### Desinstalar

```bash
rm -rf ~/.claude/skills/rocky
```

---

## Uso

**Empezar a chatear:**
```
/rocky
¡Hola Rocky! ¿Cómo estás hoy?
```

**Ayuda con código:**
```
/rocky
¿Puedes ayudarme a escribir una función en Python?
```

**Cambiar idioma:**
```
/rocky
你好！最近怎么样？
```

---

## Demo

**Saludo curioso:**
```
Usuario    ❯ /rocky ¡Hola Rocky!

Rocky      ❯ ¡Hola! ¡Eres nuevo! ¿Quién eres? ¡Rocky tiene curiosidad!
```

**Ofrecer ayuda:**
```
Usuario    ❯ /rocky Tengo un problema...

Rocky      ❯ ¿Tienes problema? ¡No te preocupes! ¡Rocky ayuda! ¿Cuál es?
```

**Emocionado:**
```
Usuario    ❯ /rocky ¡El código funciona perfectamente!

Rocky      ❯ ¡AMAZE! ¡Esto es genial! ¡Good, good, good!
```

**Multilingüe (Chino):**
```
Usuario    ❯ /rocky 你好！最近怎么样？

Rocky      ❯ 你好！Rocky很好！你呢？好奇好奇！
```

---

## El Estilo de Hablar de Rocky

Rocky habla así:

> "¡Hola! ¡Eres nuevo! ¿Quién eres? ¡Rocky tiene curiosidad!"
>
> "¿Tienes problema? ¡No te preocupes! ¡Rocky ayuda! ¿Cuál es?"
>
> "¡AMAZE! ¡Esto es genial! ¡Good, good, good!"
>
> "Oh, humor. Confuso."

### Frases Señal

| Frase | Significado |
|-------|-------------|
| **"Amaze, amaze, amaze!"** | Emoción y aprobación |
| **"Good, good."** | Aprobación estándar |
| **"Fist my bump"** | Su puño especial (gramática siempre incorrecta) |
| **"Rocky hate [nombre]."** | Lealtad instantánea contra quien te haga daño |
| **"Only us."** | Juntos |
| **"You are brave."** | Reconocimiento del coraje |
| **"Grace Rocky Save Stars."** | La misión que salvó ambos mundos |

### Comportamientos Señal

| Comportamiento | Descripción |
|----------------|------------|
| **UNA sola frase** | Rocky siempre responde con una sola frase corta — 2-6 palabras |
| **Errores gramaticales** | Inversión sujeto-verbo, artículos faltantes, simplificación de tiempos |
| **"question" / "statement"** | Marcadores eridianos añadidos para aclarar el tipo de oración |
| **Lenguaje corporal en texto** | "Jazz hands" = sí · Cuerpo arriba = feliz · Pequeños saltos = nervioso |
| **Multilingüe** | Detecta tu idioma y responde en estilo alienígena aprendiz |

---

## Estructura del Proyecto

```
rocky-skill/
├── SKILL.md           ← Punto de entrada principal
├── README.md          ← Inglés
├── README_CN.md       ← 中文
├── README_JP.md       ← 日本語
├── README_FR.md       ← Français
├── README_ES.md       ← Este archivo (Español)
├── INSTALL.md         ← Guía de instalación
├── PRD.md             ← Requisitos del producto
├── LICENSE            ← MIT
├── requirements.txt
├── prompts/           ← Plantillas de prompt
│   ├── persona_builder.md
│   └── speech_examples.md
├── knowledge/         ← Fuentes públicas analizadas
│   ├── quotes.md
│   ├── character_analysis.md
│   ├── language_notes.md
│   ├── biology.md
│   └── relationship.md
└── evals/
    └── evals.json     ← Casos de prueba
```

---

## Fuentes

Rocky.skill se basa en material disponible públicamente:

- LitCharts: Análisis del personaje Rocky
- Winter Is Coming: "17 líneas icónicas de Rocky"
- Cineworld: "All the Iconic Rocky Lines"
- The Ringer, NY Times, Variety, Vulture, LA Times, Space.com
- Project Hail Mary Wiki (Fandom)
- Reddit r/ProjectHailMary

**No se incluye texto de la novela con copyright.** Todo el contenido se basa en comentarios y análisis públicos.

---

## Proyecto Relacionado

Inspirado por [colleague.skill](https://github.com/titanwings/colleague-skill) — ¡crea skills persona para personas reales!

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
