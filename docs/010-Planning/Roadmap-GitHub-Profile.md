---
id: ROADMAP-001
type: roadmap
status: review
project: jhm1909-profile
tags: [github-profile, readme, branding]
created: 2026-03-03
---

# 🗺️ Roadmap: GitHub Profile README — "Capy" Edition

> **Mục tiêu**: Biến `jhm1909/jhm1909` README thành profile GitHub hoành tráng nhất có thể, Dark Futuristic aesthetic.

---

## Phase 1: Core Foundation ⚡ (Ngay lập tức)

> Impact cao nhất, triển khai đầu tiên.

| # | Deliverable | Tool/Service | Thời gian |
|---|-------------|-------------|-----------|
| 1.1 | Animated header banner | `capsule-render` (waving, gradient cyan) | 5 min |
| 1.2 | Typing SVG intro | `readme-typing-svg` | 5 min |
| 1.3 | About Me section | Markdown + emoji | 5 min |
| 1.4 | Tech Stack icons | `skill-icons` + `shields.io` | 10 min |
| 1.5 | GitHub Stats cards | `github-readme-stats` (tokyonight theme) | 5 min |
| 1.6 | Streak Stats | `github-readme-streak-stats` | 5 min |
| 1.7 | Contact badges | `shields.io` (Email) | 5 min |

**Tổng**: ~40 min

---

## Phase 2: Visual Excellence 🎨 (Trong ngày)

> Nâng tầm visual, tạo sự khác biệt.

| # | Deliverable | Tool/Service | Thời gian |
|---|-------------|-------------|-----------|
| 2.1 | GitHub Trophies | `github-profile-trophy` | 5 min |
| 2.2 | Activity Graph | `github-readme-activity-graph` | 5 min |
| 2.3 | Snake Contribution Graph | `Platane/snk` + GitHub Actions | 15 min |
| 2.4 | Profile views counter | `komarev/github-profile-views-counter` | 2 min |
| 2.5 | Animated footer | `capsule-render` (footer section) | 5 min |

**Tổng**: ~32 min

---

## Phase 3: Automation & Dynamic 🤖 (Nâng cao)

> Dynamic content, auto-update, cực kỳ ấn tượng.

| # | Deliverable | Tool/Service | Thời gian |
|---|-------------|-------------|-----------|
| 3.1 | 3D Contribution Graph | `github-profile-3d-contrib` + Actions | 15 min |
| 3.2 | Spotify Now Playing | Vercel deploy + Spotify API | 30 min |
| 3.3 | Lowlighter Metrics | `lowlighter/metrics` + Actions | 20 min |
| 3.4 | Recent activity feed | `github-activity-readme` | 10 min |

**Tổng**: ~75 min

---

## Timeline Tổng

```
Phase 1 (Core)       ████████████░░░░░░░░  40 min
Phase 2 (Visual)     ████████░░░░░░░░░░░░  32 min  
Phase 3 (Automation) ████████████████░░░░  75 min
─────────────────────────────────────────
TOTAL                                     ~2.5 hrs
```

---

## Milestones

- **M1**: README hoàn chỉnh với header, stats, tech stack → **Phase 1 done**
- **M2**: Profile đầy đủ visual effects (snake, trophy, graph) → **Phase 2 done**
- **M3**: Dynamic content auto-update (Spotify, 3D, metrics) → **Phase 3 done**

---

## Risk & Mitigation

| Risk | Impact | Mitigation |
|------|--------|------------|
| GitHub Actions quota limits | Snake/3D graph không chạy | Dùng cron thưa hơn (1x/ngày) |
| Third-party service down | Broken images | Dùng các service ổn định, có fallback |
| Profile views counter spam | Số liệu không chính xác | Dùng `komarev` (reliable) |
| Spotify API token expire | Widget không hoạt động | Refresh token auto-renewal |
