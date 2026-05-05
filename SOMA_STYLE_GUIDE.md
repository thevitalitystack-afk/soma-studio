# SOMA Studio — Dark Theme Style Guide

## Overview

This document outlines the modern dark theme design system implemented for the SOMA Studio dashboard, focusing on clean padding, professional spacing, and visual hierarchy.

---

## Color Palette

### Base Colors
| Variable | Value | Usage |
|----------|-------|-------|
| `--bg` | `#0a0a0f` | Primary background |
| `--bg-elevated` | `#11111a` | Elevated surfaces |
| `--bg-card` | `#161622` | Card backgrounds |
| `--surface` | `#1e1e28` | UI surfaces |

### Borders & Dividers
| Variable | Value | Usage |
|----------|-------|-------|
| `--border` | `#2a2a35` | Component borders |
| `--border-soft` | `#22222c` | Subtle borders |
| `--divider` | `rgba(255,255,255,0.03)` | Internal dividers |

### Typography
| Variable | Value | Usage |
|----------|-------|-------|
| `--text` | `#e8e6ed` | Primary text |
| `--text-secondary` | `#a8a4af` | Secondary text |
| `--text-tertiary` | `#7a7680` | Tertiary text |
| `--text-muted` | `#5a565f` | Disabled/muted |

### Brand Accents
| Variable | Value | Usage |
|----------|-------|-------|
| `--accent` | `#c8a878` | Primary brand color |
| `--accent-strong` | `#d6b88a` | Hover/active states |
| `--accent-soft` | `rgba(200,168,120,0.12)` | Backgrounds |
| `--accent-line` | `rgba(200,168,120,0.25)` | Borders/highlights |

### Status Colors
| Variable | Value | Usage |
|----------|-------|-------|
| `--status-active` | `#a3ffb4` | Active/running |
| `--status-idle` | `#ffb968` | Idle/waiting |
| `--status-off` | `#ff6b6b` | Off/disabled |
| `--status-working` | `#7fb8ff` | Working/in progress |

---

## Spacing Scale

| Size | Value | Usage |
|------|-------|-------|
| `--space-xs` | `4px` | Tight spacing within components |
| `--space-sm` | `8px` | Small gaps, icon spacing |
| `--space-md` | `12px` | Medium gaps, between related items |
| `--space-lg` | `16px` | Large gaps, section spacing |
| `--space-xl` | `20px` | Between major sections |
| `--space-2xl` | `24px` | Page section margins |
| `--space-3xl` | `32px` | Major section separation |

---

## Typography

### Font Stack
```css
/* Primary */
font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Inter", sans-serif;

/* Serif headings */
font-family: "Fraunces", Georgia, serif;

/* Monospace for labels */
font-family: "JetBrains Mono", monospace;
```

### Headings
| Element | Size | Weight | Letter-spacing |
|---------|------|--------|----------------|
| h1 | 28px | 300 | -0.015em |
| Agent names | 18px | 300 | -0.01em |

### Body Text
| Element | Size | Color |
|---------|------|-------|
| Primary | 14px | `--text` |
| Secondary | 13px | `--text-secondary` |
| Labels | 10-11px | `--text-tertiary` |

---

## Components

### Agent Cards

**Structure:**
```
┌─────────────────────────────────┐
│ Header                         ●│  ← status badge
│   Name                         │
│   Role                         │
├─────────────────────────────────┤
│ Progress                       │  ← progress bar
└─────────────────────────────────┘
```

**Padding:** `var(--space-xl)` (20px)
**Border-radius:** `var(--radius-lg)` (18px)
**Hover lift:** `translateY(-2px)`

### Stat Pills

**Padding:** `var(--space-lg)` (20px)
**Border-radius:** `var(--radius-md)` (14px)
**Text alignment:** Center

### Status Badges

**Padding:** `var(--space-xs)` `var(--space-sm)` (4px 8px)
**Border-radius:** 20px
**Font:** "JetBrains Mono", 11px, uppercase

---

## Layout

### Page Structure
```
┌─────────────────────────────────┐
│ Header                         │  ← 64px height
├─────────────────────────────────┤
│ Stats Bar                      │  ← 4 rows of pills
├─────────────────────────────────┤
│ Agents Grid                    │  ← responsive grid
│   ┌──────┐ ┌──────┐ ┌──────┐   │
│   │ Card │ │ Card │ │ Card │   │
│   └──────┘ └──────┘ └──────┘   │
└─────────────────────────────────┘
```

### Grid Configuration
- **Desktop:** `repeat(auto-fill, minmax(280px, 1fr))`
- **Gap:** `var(--space-xl)` (20px)
- **Mobile:** Single column, gap `var(--space-lg)` (16px)

---

## Improvements Over Previous Version

### Padding Fixes
1. **Consistent card padding:** Standardized to `var(--space-xl)` (20px)
2. **Header spacing:** Added proper margin-bottom to title and subtitle
3. **Progress bar spacing:** Added `var(--space-lg)` margin above progress bars
4. **Section gutters:** Consistent `var(--space-3xl)` (32px) between sections

### Spacing Refinements
1. **Vertical rhythm:** Established clear spacing scale with consistent increments
2. **Grid gaps:** Unified gap sizing across all grid layouts
3. **Component breathing room:** Adequate padding prevents cramped appearance

### Dark Theme Enhancements
1. **Layered backgrounds:** Multiple background levels create depth
2. **Subtle gradients:** Soft radial gradients add dimension without distraction
3. **Status color backgrounds:** Semi-transparent status colors for context
4. **Border hierarchy:** Two-level border system (strong/soft) for visual flow

---

## Usage

To use this dark theme:

1. Include the CSS variables in your stylesheet
2. Reference the spacing scale variables
3. Use the component classes as patterns
4. Follow the responsive breakpoints

```html
<!-- Example agent card -->
<div class="agent-card is-active">
  <div class="agent-header">
    <div>
      <div class="agent-name">Pixie</div>
      <div class="agent-role">Ideation Engine</div>
    </div>
    <span class="status-badge working">
      <span class="status-dot"></span>
      working
    </span>
  </div>
  <div class="progress-container">
    <div class="progress-bar">
      <div class="progress-fill" style="width: 60%"></div>
    </div>
  </div>
</div>
```

---

## File Reference

- **Main Dashboard:** `soma-dashboard-dark.html`
- **Style Guide:** `SOMA_STYLE_GUIDE.md` (this file)

## Discord Team Tags
To tag Atlas in Discord, always write exactly: <@1496055925822328832>
