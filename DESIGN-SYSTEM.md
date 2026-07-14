# 🎨 Design System — Tokens Reference

> Complete design token reference for the Thoughts Garden design system. Based on **Material Design 3** color roles with custom botanical extensions.

---

## 🔤 Typography System

### Font Stack

| Role | Font Family | Weights | Fallback | Import |
|---|---|---|---|---|
| **Display / Headlines** | Playfair Display | 400–900, Italic | serif | Google Fonts |
| **Body Text** | Inter | 400, 600, 700 | sans-serif | Google Fonts |
| **Handwritten** | Playwrite ID | 100–400 | cursive | Google Fonts |
| **Icons** | Material Symbols Outlined | Variable (100–700) | — | Google Fonts |

### Font Family Tokens (Tailwind Config)

```javascript
fontFamily: {
    sans: ["Playfair Display", "serif"],        // Default text
    "display-lg": ["Playfair Display", "serif"], // Large display
    "body-md": ["Inter", "sans-serif"],          // Body medium (Albums)
    "body-lg": ["Inter", "sans-serif"],          // Body large (Albums)
    "headline-lg": ["Playfair Display", "serif"],// Headlines
    "headline-md": ["Playfair Display", "serif"],// Sub-headlines
    "label-caps": ["Playfair Display", "serif"], // Uppercase labels
    handwritten: ["Playwrite ID", "cursive"]     // Personal notes
}
```

### Google Fonts Import URLs

```html
<!-- Thoughts Garden (Playfair + Playwrite ID) -->
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&family=Playwrite+ID:wght@100..400&display=swap" rel="stylesheet">

<!-- Albums Page (Playfair + Inter) -->
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&family=Inter:wght@400;600;700&display=swap" rel="stylesheet">

<!-- Material Icons -->
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&display=block" rel="stylesheet">
```

---

## 🎨 Color Palette — Full Token Map

### Primary Colors — Forest Green Family

| Token | Hex | Role |
|---|---|---|
| `primary` | `#154212` | Primary text, key CTA actions |
| `on-primary` | `#ffffff` | Text on primary backgrounds |
| `primary-container` | `#2d5a27` | Card backgrounds, elevated containers |
| `on-primary-container` | `#9dd090` | Text on primary containers |
| `primary-fixed` | `#bcf0ae` | Light fixed accents, tags |
| `primary-fixed-dim` | `#a1d494` | Muted green accents |
| `on-primary-fixed` | `#002201` | Text on fixed primary |
| `on-primary-fixed-variant` | `#23501e` | Variant text on fixed primary |
| `inverse-primary` | `#a1d494` | Inverse theme primary |

### Secondary Colors

#### Thoughts Garden Variant
| Token | Hex | Role |
|---|---|---|
| `secondary` | `#9a442f` | Warm terracotta — CTA buttons |
| `on-secondary` | `#ffffff` | Text on secondary |
| `secondary-container` | `#fd9076` | Warm coral containers |
| `on-secondary-container` | `#752815` | Text on secondary container |
| `secondary-fixed` | `#ffdad2` | Light warm fixed |
| `secondary-fixed-dim` | `#ffb4a2` | Dimmed warm fixed |
| `on-secondary-fixed` | `#3c0700` | Text on fixed secondary |
| `on-secondary-fixed-variant` | `#7c2d1a` | Variant text |

#### Albums Page Variant
| Token | Hex | Role |
|---|---|---|
| `secondary` | `#8a765d` | Warm gold/brown |
| `secondary-container` | `#f5ebd6` | Cream container |
| `on-secondary-container` | `#5c4a37` | Brown text |
| `secondary-fixed` | `#faf5ea` | Very light cream |
| `secondary-fixed-dim` | `#e6dec9` | Muted cream |

### Tertiary Colors — Neutral Gray
| Token | Hex | Role |
|---|---|---|
| `tertiary` | `#383a38` | Dark neutral text |
| `on-tertiary` | `#ffffff` | Text on tertiary |
| `tertiary-container` | `#4f514e` | Dark containers |
| `on-tertiary-container` | `#c3c3c0` | Light text on dark |
| `tertiary-fixed` | `#e2e3df` | Light neutral fixed |
| `tertiary-fixed-dim` | `#c6c7c3` | Muted neutral |
| `on-tertiary-fixed` | `#1a1c1a` | Dark text on fixed |
| `on-tertiary-fixed-variant` | `#454745` | Variant dark text |

### Surface and Background
| Token | Hex | Role |
|---|---|---|
| `background` | `#fbf9f8` | Page background — warm off-white |
| `on-background` | `#1b1c1c` | Primary text |
| `surface` | `#fbf9f8` | Card surfaces |
| `on-surface` | `#1b1c1c` | Text on surfaces |
| `on-surface-variant` | `#42493e` | Secondary/muted text |
| `surface-variant` | `#e4e2e2` | Variant surface |
| `surface-dim` | `#dbd9d9` | Dimmed surface |
| `surface-bright` | `#fbf9f8` | Bright surface |
| `surface-tint` | `#3b6934` | Tint overlay color |

### Surface Containers (Elevation)
| Token | Hex | Elevation Level |
|---|---|---|
| `surface-container-lowest` | `#ffffff` | Level 0 — Pure white |
| `surface-container-low` | `#f5f3f3` | Level 1 |
| `surface-container` | `#efeded` | Level 2 — Default |
| `surface-container-high` | `#eae8e7` | Level 3 |
| `surface-container-highest` | `#e4e2e2` | Level 4 |

### Utility Colors
| Token | Hex | Role |
|---|---|---|
| `outline` | `#72796e` | Borders, dividers |
| `outline-variant` | `#c2c9bb` | Subtle borders |
| `error` | `#ba1a1a` | Error states |
| `on-error` | `#ffffff` | Text on error |
| `error-container` | `#ffdad6` | Error container |
| `on-error-container` | `#93000a` | Text on error container |
| `inverse-surface` | `#303030` | Dark inverse surface |
| `inverse-on-surface` | `#f2f0f0` | Light text on inverse |

---

## 🎭 Accent Colors — Special Effects

These are **not part of the M3 token system** but are used for premium visual effects:

| Color Name | Hex | Where Used |
|---|---|---|
| Rose Gold | `#d98270` | Conic gradient glow — streak 1 |
| Cream Glow | `#eed8a1` | Conic gradient glow — streak 1 |
| Sage Green | `#6b8f71` | Conic gradient glow — streak 2 |
| Light Sage | `#abc9a5` | Conic gradient glow — streak 2 |
| Scribble Background | `#fdfcf7` | Notepad card backgrounds |
| Scribble Border | `#f2edd9` | Notepad card borders |
| Dog-Ear Fold | `#eae4cd` | Corner fold on scribble cards |
| Focus Ring | `rgba(161, 212, 148, 0.4)` | Accessibility focus glow |
| Focus Border | `rgba(91, 148, 77, 0.6)` | Accessibility focus border |
| Ruled Paper Line | `rgba(59, 105, 52, 0.08)` | Notebook ruled lines |

---

## 📐 Spacing System

| Token | Value | CSS Usage |
|---|---|---|
| `unit` | `8px` | `p-unit`, base spacing |
| `stack-sm` | `12px` | `gap-stack-sm`, small gaps |
| `stack-md` | `24px` | `gap-stack-md`, medium gaps |
| `stack-lg` | `48px` | `pb-stack-lg`, section spacing |
| `gutter` | `24px` | `gap-gutter`, column gaps |
| `margin-mobile` | `20px` | `px-margin-mobile` |
| `margin-desktop` | `64px` | `px-margin-desktop` |
| `container-max` | `1140px` | `max-w-container-max` |

---

## 🔲 Border Radius Tokens

| Token | Value | Visual |
|---|---|---|
| `rounded` (default) | `1rem` — 16px | Standard cards |
| `rounded-lg` | `2rem` — 32px | Large containers |
| `rounded-xl` | `3rem` — 48px | Hero sections |
| `rounded-full` | `9999px` | Pills, avatars |

---

## 🌫️ Glassmorphism Recipes

### Standard Glass Card
```css
background: rgba(255, 255, 255, 0.45);
backdrop-filter: blur(20px);
-webkit-backdrop-filter: blur(20px);
border: 1px solid rgba(255, 255, 255, 0.25);
```

### Navbar (Scrolled State)
```css
background-color: rgba(251, 249, 248, 0.95);
box-shadow: 0 4px 20px rgba(0,0,0,0.02);
border-color: rgba(194, 201, 187, 0.4);
```

### Scribble Note
```css
background-color: #fdfcf7;
border: 1px solid #f2edd9;
box-shadow: 0 4px 15px rgba(161, 142, 107, 0.08);
```

---

## ⏱️ Animation Easing

| Name | Curve | Usage |
|---|---|---|
| **Garden Ease** | `cubic-bezier(0.16, 1, 0.3, 1)` | All reveals, hovers, transitions |
| **Linear** | `linear` | Marquee loop, glow rotation |
| **Ease-in-out** | `ease-in-out` | Leaf sway animation |

---

## 📋 Complete Tailwind Config

```javascript
tailwind.config = {
    darkMode: "class",
    theme: {
        extend: {
            colors: {
                "primary": "#154212",
                "primary-container": "#2d5a27",
                "primary-fixed": "#bcf0ae",
                "primary-fixed-dim": "#a1d494",
                "secondary": "#9a442f",
                "background": "#fbf9f8",
                "surface": "#fbf9f8",
                "on-surface": "#1b1c1c",
                "on-surface-variant": "#42493e",
                "outline": "#72796e",
                "outline-variant": "#c2c9bb",
                "surface-tint": "#3b6934",
                // ... 40+ tokens total
            },
            borderRadius: {
                DEFAULT: "1rem",
                lg: "2rem",
                xl: "3rem",
                full: "9999px"
            },
            spacing: {
                "unit": "8px",
                "stack-sm": "12px",
                "stack-md": "24px",
                "stack-lg": "48px",
                "gutter": "24px",
                "margin-mobile": "20px",
                "margin-desktop": "64px",
                "container-max": "1140px"
            },
            fontFamily: {
                sans: ["Playfair Display", "serif"],
                handwritten: ["Playwrite ID", "cursive"]
            }
        }
    }
}
```
