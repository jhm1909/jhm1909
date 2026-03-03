---
id: PRD-001
type: prd
status: review
project: jhm1909-profile
tags: [github-profile, readme, branding, developer-portfolio]
created: 2026-03-03
---

# 📋 PRD: GitHub Profile README — "Capy" | Dark Futuristic Edition

## 1. Tổng Quan

**Sản phẩm**: GitHub Profile README cho user `jhm1909`  
**Persona**: "Capy" — Full-Stack Developer, Go-first mindset  
**Theme**: Dark Futuristic (Cyberpunk, neon cyan trên nền tối `#0d1117`)  
**Mục tiêu**: Profile GitHub ấn tượng nhất, khiến mọi developer — mới hay lâu năm — đều "WOW"

---

## 2. Thông Tin Cá Nhân

| Field | Value |
|-------|-------|
| Display Name | **Capy** |
| Role | Full-Stack Developer |
| Primary Stack | Go, TypeScript, React, Next.js, Docker, PostgreSQL, Redis |
| Contact | jeonghamin1909@gmail.com |
| Theme | Dark Futuristic (`#0d1117` bg, `#00d4ff` accent, `#c9d1d9` text) |
| Spotify | Có — Tích hợp Now Playing widget |

---

## 3. Thiết Kế Visual

### 3.1 Color Palette — "Midnight Cyan"

```
Background:  #0d1117  (GitHub Dark default)
Primary:     #00d4ff  (Neon Cyan — main accent)
Secondary:   #bb86fc  (Purple — secondary accent)
Accent Hot:  #ff6b6b  (Red/Pink — highlights)
Text:        #c9d1d9  (Soft white)
Subtext:     #8b949e  (Muted gray)
```

### 3.2 Stats Card Theme: `tokyonight`
Tất cả cards dùng cùng theme để đồng bộ visual.

---

## 4. Cấu Trúc README (Top → Bottom)

### Section 1: Animated Header
- **Tool**: `capsule-render`
- **Type**: `waving`
- **Text**: `Welcome to Capy's Universe`
- **Colors**: Gradient `#00d4ff` → `#bb86fc`
- **Height**: 300px
- **Font**: Monoton (futuristic)

### Section 2: Typing SVG
- **Tool**: `readme-typing-svg`
- **Lines**:
  - `> Full-Stack Developer 🚀`
  - `> Go | TypeScript | React | Next.js`
  - `> Building the future, one commit at a time`
- **Color**: `#00d4ff`
- **Background**: Transparent
- **Speed**: vừa phải, loop vô hạn

### Section 3: About Me
- **Style**: Markdown với emoji
- **Nội dung**:
  - 🔭 Currently working on...
  - 🌱 Currently learning...
  - 💬 Ask me about Go, System Design, APIs
  - ⚡ Fun fact: ...
- **Tone**: Professional nhưng friendly, personality-driven

### Section 4: Tech Stack
- **Tool**: `skill-icons` (tanzpfun/skill-icons)
- **Icons**: Go, TypeScript, JavaScript, React, NextJS, NodeJS, Docker, PostgreSQL, Redis, Git, GitHub, Linux, VSCode, TailwindCSS, HTML, CSS
- **Layout**: Centered, per_line=8
- **Theme**: Dark

### Section 5: GitHub Stats
- **Tool**: `github-readme-stats`
- **Cards** (2 cards side-by-side):
  - Stats card (commits, PRs, issues, stars)
  - Top Languages card (layout: compact)
- **Theme**: `tokyonight`
- **Border**: Không
- **Show icons**: Có

### Section 6: Streak Stats
- **Tool**: `github-readme-streak-stats`
- **Theme**: `tokyonight`
- **Border**: Không

### Section 7: Activity Graph
- **Tool**: `github-readme-activity-graph`
- **Background**: `#0d1117`
- **Line color**: `#00d4ff`
- **Point color**: `#bb86fc`
- **Area**: Có (fill dưới line)

### Section 8: GitHub Trophies
- **Tool**: `github-profile-trophy`
- **Theme**: `algolia` hoặc `darkhub`
- **Columns**: 7
- **Row**: 1
- **No-frame**: Có
- **No-bg**: Có

### Section 9: Snake Contribution Graph
- **Tool**: `Platane/snk`
- **GitHub Action**: Chạy daily
- **Output**: SVG animation (dark mode)
- **Colors**: GitHub dark palette

### Section 10: 3D Contribution Graph
- **Tool**: `github-profile-3d-contrib`
- **GitHub Action**: Chạy daily
- **Profile**: `night-green` hoặc `night-view`

### Section 11: Spotify Now Playing
- **Deploy**: Vercel
- **Tool**: `novatorem/spotify-github-profile` hoặc tương tự
- **Theme**: Dark, matching palette

### Section 12: Profile Views Counter
- **Tool**: `komarev/github-profile-views-counter`
- **Color**: `#00d4ff`
- **Style**: `for-the-badge`

### Section 13: Contact & Social
- **Style**: Shields.io badges
- **Links**: Email badge
- **Colors**: Matching theme

### Section 14: Animated Footer
- **Tool**: `capsule-render`
- **Type**: `waving`
- **Section**: `footer`
- **Colors**: Gradient matching header

---

## 5. GitHub Actions Workflows

### 5.1 Snake Contribution
- **File**: `.github/workflows/snake.yml`
- **Schedule**: `0 0 * * *` (mỗi ngày lúc 00:00 UTC)
- **Output**: `dist/github-snake-dark.svg`

### 5.2 3D Contribution
- **File**: `.github/workflows/profile-3d.yml`
- **Schedule**: `0 1 * * *` (mỗi ngày lúc 01:00 UTC)
- **Output**: `profile-3d-contrib/profile-night-green.svg`

### 5.3 Metrics (Tùy chọn Phase 3)
- **File**: `.github/workflows/metrics.yml`
- **Schedule**: `0 2 * * *`

---

## 6. Feature Prioritization (MoSCoW)

| Priority | Feature | Justification |
|----------|---------|---------------|
| **MUST** | Header animation, Typing SVG, About Me, Tech Stack, Stats, Streak | Core identity & visual impact |
| **MUST** | GitHub Trophies, Activity Graph | Credibility & engagement proof |
| **SHOULD** | Snake Graph, 3D Graph, Footer animation | WOW factor, unique differentiation |
| **SHOULD** | Profile views counter, Contact badges | Social proof & accessibility |
| **COULD** | Spotify Now Playing | Personal touch, fun factor |
| **COULD** | Metrics dashboard, Activity feed | Advanced data visualization |

---

## 7. Success Metrics

| Metric | Target |
|--------|--------|
| Thời gian load tất cả widgets | < 3s |
| Số widgets hiển thị đúng | 100% (0 broken images) |
| GitHub Actions chạy thành công | 100% |
| Visual consistency (theme đồng bộ) | Tất cả cards cùng `tokyonight` |
| First impression reaction | "WOW" từ dev mới lẫn senior |

---

## 8. Liên Kết

- [[Analysis-GitHub-Profile-README]] — Research insights
- [[Roadmap-GitHub-Profile]] — Implementation timeline
