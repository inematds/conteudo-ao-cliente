# conteudo-ao-cliente

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

[![From content to client](guia/assets/banner-en.jpg)](https://inematds.github.io/conteudo-ao-cliente/guia/en/)

## What it is

This page brings together five pieces that already exist separately across INEMA and shows how they fit together. There are four free tools that run in your computer’s terminal with the help of Claude Code (an AI assistant that works there), plus a short course. They’re for people who create content—on their own or at a small company—and lose track of things between choosing a topic, producing, publishing, and replying. Each piece handles one step: finding the topic of the day, seeing what has already worked on your channels, building a carousel, delivering the material to people who comment, and handing the rest of the routine to an agent. Each has its own guide and works on its own. You can use just one or all five together.

## 📖 User guide

Full page (what each piece does + step-by-step instructions): **https://inematds.github.io/conteudo-ao-cliente/guia/en/**

## The 5 pieces

| # | Piece | What it does | Guide |
|---|---|---|---|
| 1 | 📡 radar-pautas | Reads ~20 AI news sites and returns the 6 hottest topics of the day, with verified links | [guide](https://inematds.github.io/radar-pautas/guia/en/) |
| 2 | 📈 muse-canais | Finds recent videos on your YouTube channels that are 2× above normal and suggests 8 ideas | [guide](https://inematds.github.io/muse-canais/guia/en/) |
| 3 | 🖼️ carrossel-inema | Claude Code skill: cover, slides, “comment WORD,” and 3 stories in the right dimensions | [guide](https://inematds.github.io/carrossel-inema/guia/en/) |
| 4 | 💬 lead-comenta | Free resource page for people who comment, plus ready-to-use reply messages | [guide](https://inematds.github.io/lead-comenta/guia/en/) |
| 5 | 🧹 Course | Hand the tedious work to an agent — 8 lessons, through chat or the terminal | [course](https://inematds.github.io/trabalho-chato-ao-agente-v72/en/) |

## The process, from start to finish

| Step | What | Command | Who does it |
|---|---|---|---|
| 1 | Find the topic of the day | `python3 radar.py --dry` (in radar-pautas) | ⚙️ script |
| 2 | See what has already worked | `python3 muse.py --ideias` (in muse-canais) | ⚙️ script + 🤖 Claude Code |
| 3 | Make the carousel | Ask Claude Code with the carrossel-inema skill enabled | 🤖 Claude Code |
| 4 | Check the slides | `python3 scripts/checa.py <pasta> <roteiro.json>` | ⚙️ script |
| 5 | Prepare the material for people who comment | `python3 lead.py nova PALAVRA --tema "..." --fonte <url>` | 🤖 Claude Code |
| 6 | Approve and post | You review everything and publish | 🧠 you |
| 7 | Delegate the routine | Follow the trabalho-chato-ao-agente course | 🧠 you |

This repository contains only the page. Each tool’s code is in its own repository.

---

[INEMA.CLUB](https://inema.club)
