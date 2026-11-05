# conteudo-ao-cliente

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

[![Do conteúdo ao cliente](guia/assets/banner.jpg)](https://inematds.github.io/conteudo-ao-cliente/guia/)

## O que é

Esta página junta cinco peças que já existem separadas no INEMA e mostra como elas se encaixam. São quatro ferramentas gratuitas, que rodam no terminal do seu computador com a ajuda do Claude Code (um assistente de IA que trabalha ali), e um curso curto. Servem para quem cria conteúdo (sozinho ou numa empresa pequena) e se perde entre escolher o assunto, produzir, publicar e responder. Cada peça cuida de uma etapa: achar a pauta do dia, ver o que já funcionou nos seus canais, montar o carrossel, entregar o material para quem comenta e passar o resto da rotina para um agente. Cada uma tem o seu guia e funciona sozinha. Você pode usar uma só ou as cinco juntas.

## 📖 Guia de uso

Página completa (o que cada peça faz + passo a passo): **https://inematds.github.io/conteudo-ao-cliente/guia/**

## As 5 peças

| # | Peça | O que faz | Guia |
|---|---|---|---|
| 1 | 📡 radar-pautas | Lê ~20 sites de notícias de IA e devolve as 6 pautas mais quentes do dia, com link conferido | [guia](https://inematds.github.io/radar-pautas/guia/) |
| 2 | 📈 muse-canais | Acha os vídeos recentes 2× acima do normal dos seus canais do YouTube e propõe 8 ideias | [guia](https://inematds.github.io/muse-canais/guia/) |
| 3 | 🖼️ carrossel-inema | Skill do Claude Code: capa, slides, "comenta PALAVRA" e 3 stories no tamanho certo | [guia](https://inematds.github.io/carrossel-inema/guia/) |
| 4 | 💬 lead-comenta | Página do material grátis de quem comenta + textos de resposta prontos | [guia](https://inematds.github.io/lead-comenta/guia/) |
| 5 | 🧹 Curso | Entregue o trabalho chato a um agente — 8 aulas, pelo chat ou pelo terminal | [curso](https://inematds.github.io/trabalho-chato-ao-agente-v72/) |

## O processo, do início ao fim

| Passo | O quê | Comando | Quem faz |
|---|---|---|---|
| 1 | Achar a pauta do dia | `python3 radar.py --dry` (no radar-pautas) | ⚙️ script |
| 2 | Ver o que já funcionou | `python3 muse.py --ideias` (no muse-canais) | ⚙️ script + 🤖 Claude Code |
| 3 | Fazer o carrossel | pedir ao Claude Code com a skill carrossel-inema ligada | 🤖 Claude Code |
| 4 | Conferir os slides | `python3 scripts/checa.py <pasta> <roteiro.json>` | ⚙️ script |
| 5 | Preparar o material de quem comenta | `python3 lead.py nova PALAVRA --tema "..." --fonte <url>` | 🤖 Claude Code |
| 6 | Aprovar e postar | você olha tudo e publica | 🧠 você |
| 7 | Delegar a rotina | seguir o curso trabalho-chato-ao-agente | 🧠 você |

Este repositório tem só a página. O código de cada ferramenta está no repositório dela.

---

[INEMA.CLUB](https://inema.club)
