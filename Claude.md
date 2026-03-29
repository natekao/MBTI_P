# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains two independent projects:

1. **MBTI 測驗網站** — A single-file Traditional Chinese MBTI personality quiz and introduction site (`index.html`). Pure HTML/CSS/JS with no build tools or dependencies.
2. **冒險故事** — An ongoing adventure story written collaboratively in `故事.md`.

## Running the Website

Open `index.html` directly in a browser — no server or build step required.

## Story Writing Convention

In `故事.md`, lines beginning with `#標題` are **story direction prompts**, not Markdown headings. They guide what Claude should write next. When asked to continue the story:

- Write prose **below** the `#標題` line, keeping the heading in place
- Target word count per section is specified by the user (e.g. 100字、200字)
- Maintain consistency with character profiles below

### Character Rules

- **小明**：3歲起由阿姨撫養的孤兒，開朗活潑。故事中不能出現「媽媽」，只能說「阿姨」。
- **小花**：小明的鄰居，內向，暗戀小明但小明從未察覺。
- **美美**：小花的好朋友，女性，與小花同齡，個性開朗活潑、愛講笑話，常能炒熱氣氛。
- **祐祐**：足球隊的國二學長，14歲，話多外向，是學校的風雲人物，與各方關係都很好。
- **岑岑**：10歲女孩，個性木訥，與大家關係普通，但內心深處渴望交到好朋友；擅長織布、繪畫與色彩應用。

## Key Files

| File | Purpose |
|------|---------|
| `index.html` | MBTI website (all-in-one) |
| `故事.md` | Active story manuscript |
| `計畫.md` | Combined character + story overview |

## Installed Plugins

- **nano-banana** (`.claude/plugins/nano-banana/`) — AI image generation via Gemini API. Requires `nano-banana` CLI and `GEMINI_API_KEY` set in `~/.nano-banana/.env`. Run `/init` to set up the CLI if not already installed.
