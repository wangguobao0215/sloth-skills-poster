---
name: sloth-skills-poster
description: >-
  Generate and maintain the "树懒老K AI技能海报" — a single-page HTML poster showcasing
  the Sloth-Role-Eido skill family (CPQ, PSC, Sales, StratAlign, SMM, etc.) with skill
  cards, audience tags, pain points, feature highlights, and links to demos and GitHub repos.
  Use when user asks to create, update, or regenerate the skill poster, skill showcase,
  skill catalog page, or marketing landing page for the Sloth skill family.
---

# Sloth-Skills-Poster

Generate and maintain the 树懒老K AI技能矩阵 single-page HTML poster.

## What This Skill Does

Produces a self-contained HTML file (`index.html`) that renders a mobile-friendly poster card showcasing all Sloth-Role-Eido skills. Each skill card includes: icon, name, target audience, pain point, feature summary, and links to demo video and GitHub repo.

## Design Spec

- **Layout**: Single centered card (420px wide), mobile-friendly
- **Color palette**: 雾霁蓝 (Misty Blue) — `#4a80a8` primary, `#2a3e50` text, `#e8eef5` background
- **Typography**: System font stack with PingFang SC / Microsoft YaHei fallback
- **Card style**: Frosted glass effect (`backdrop-filter: blur`), hover elevation
- **Footer**: Open source badge, slogan "慢一点，深一度"

## How to Add a New Skill Card

Insert a new `<div class="skill-card">` block inside the `<div class="skills">` section:

```html
<div class="skill-card">
  <span class="skill-icon">EMOJI</span>
  <div class="skill-name">技能名称</div>
  <span class="skill-audience">目标用户角色</span>
  <div class="skill-pain">痛点：一句话描述</div>
  <div class="skill-features">核心能力描述（2-3句话）</div>
  <div class="skill-links">
    <a href="DEMO_URL" target="_blank">观看演示</a>
    <a href="GITHUB_URL" target="_blank">GitHub</a>
  </div>
</div>
```

## Current Skills in Poster

### 新增技能
1. **产销协同智能副驾** (ProdSync) — 快消品产销协同决策参谋 · v2.3.0

### 核心技能
2. **B2B销售智能助理** (Sales) — 25+能力关系驱动完整销售周期 · v5.0
3. **售前顾问助理** (PSC) — 十二大模块售前全链路 · v2.0
4. **智能报价助手** (CPQ) — 装备制造报价 · v1.0.0
5. **战略对齐引擎** (StratAlign) — 战略落地与AI投资 · v0.5.0-beta
6. **自媒体全流程运营** (SMM) — 内容创作与多平台发布 · v1.0.0 社区版

## Files

```
sloth-skills-poster/
├── SKILL.md          # This file
├── index.html        # The poster page (self-contained HTML+CSS)
└── sloth-avatar.jpg  # Avatar image used in the poster header
```

## Usage

Open `index.html` directly in a browser, or serve it via any static file server. No build step or dependencies required.
