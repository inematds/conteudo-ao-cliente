# conteudo-ao-cliente

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

[![Del contenido al cliente](guia/assets/banner-es.jpg)](https://inematds.github.io/conteudo-ao-cliente/guia/es/)

## Qué es

Esta página reúne cinco piezas que ya existen por separado en INEMA y muestra cómo encajan. Son cuatro herramientas gratuitas que funcionan en la terminal de tu computadora con la ayuda de Claude Code (un asistente de IA que trabaja allí), y un curso corto. Sirven para quienes crean contenido (a solas o en una empresa pequeña) y se pierden entre elegir el tema, producir, publicar y responder. Cada pieza se ocupa de una etapa: encontrar el tema del día, ver qué ya funcionó en tus canales, armar el carrusel, entregar el material a quienes comentan y delegar el resto de la rutina a un agente. Cada una tiene su guía y funciona por separado. Puedes usar una sola o las cinco juntas.

## 📖 Guía de uso

Página completa (qué hace cada pieza + paso a paso): **https://inematds.github.io/conteudo-ao-cliente/guia/es/**

## Las 5 piezas

| # | Pieza | Qué hace | Guía |
|---|---|---|---|
| 1 | 📡 radar-pautas | Lee ~20 sitios de noticias sobre IA y devuelve los 6 temas más relevantes del día, con el enlace verificado | [guía](https://inematds.github.io/radar-pautas/guia/es/) |
| 2 | 📈 muse-canais | Encuentra los videos recientes de tus canales de YouTube que superan 2× su rendimiento habitual y propone 8 ideas | [guía](https://inematds.github.io/muse-canais/guia/es/) |
| 3 | 🖼️ carrossel-inema | Skill de Claude Code: portada, diapositivas, «comenta PALABRA» y 3 stories en el tamaño correcto | [guía](https://inematds.github.io/carrossel-inema/guia/es/) |
| 4 | 💬 lead-comenta | Página del material gratuito para quienes comentan + textos de respuesta listos | [guía](https://inematds.github.io/lead-comenta/guia/es/) |
| 5 | 🧹 Curso | Delega el trabajo pesado a un agente: 8 clases, por chat o por terminal | [curso](https://inematds.github.io/trabalho-chato-ao-agente-v72/es/) |

## El proceso, de principio a fin

| Paso | Qué | Comando | Quién lo hace |
|---|---|---|---|
| 1 | Encontrar el tema del día | `python3 radar.py --dry` (en radar-pautas) | ⚙️ script |
| 2 | Ver qué ya funcionó | `python3 muse.py --ideias` (en muse-canais) | ⚙️ script + 🤖 Claude Code |
| 3 | Crear el carrusel | Pedirlo a Claude Code con la skill carrossel-inema activada | 🤖 Claude Code |
| 4 | Revisar las diapositivas | `python3 scripts/checa.py <pasta> <roteiro.json>` | ⚙️ script |
| 5 | Preparar el material para quienes comentan | `python3 lead.py nova PALAVRA --tema "..." --fonte <url>` | 🤖 Claude Code |
| 6 | Aprobar y publicar | Revisas todo y lo publicas | 🧠 tú |
| 7 | Delegar la rutina | Seguir el curso trabalho-chato-ao-agente | 🧠 tú |

Este repositorio contiene solo la página. El código de cada herramienta está en su propio repositorio.

---

[INEMA.CLUB](https://inema.club)
