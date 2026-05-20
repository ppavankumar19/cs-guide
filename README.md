# CS Guide — Interactive Computer Science Learning

A collection of single-file, interactive guides to core Computer Science concepts. No frameworks, no build tools, no installation — just open an HTML file in any browser and start learning.

---

## Project Structure

```
cs-guide/
├── index.html      ← Hub page — topic selection
├── oops.html       ← Object-Oriented Programming guide (complete)
└── README.md       ← You are here
```

---

## Topics

| Topic | File | Status |
|---|---|---|
| Object-Oriented Programming | `oops.html` | ✅ Available |
| Data Structures | `ds.html` | 🔜 Coming soon |
| Algorithms | `algorithms.html` | 🔜 Coming soon |
| Computer Networks | `networks.html` | 🔜 Coming soon |
| Operating Systems | `os.html` | 🔜 Coming soon |
| Database Management | `dbms.html` | 🔜 Coming soon |
| System Design | `system-design.html` | 🔜 Coming soon |
| Python Fundamentals | `python.html` | 🔜 Coming soon |

---

## What's Inside Each Guide

Every guide follows the same structure:

- **Concept explanations** with real-world analogies
- **Syntax breakdowns** with colour-highlighted code blocks
- **Interactive simulators** — click/interact to see concepts live
- **Quiz section** — multiple choice questions across difficulty levels (basic → interview)
- **Cheatsheet** — quick reference card for the whole topic
- **Dark mode** — persisted via localStorage
- **Fully responsive** — works on mobile, tablet, desktop

---

## OOP Guide — What's Covered (`oops.html`)

8 core concepts, 8 live simulators, 50 quiz questions:

1. **Class & Object** — blueprint vs instance, tea shop simulator
2. **self** — how Python passes the current object to methods
3. **Constructor (`__init__`)** — phone setup phase simulator
4. **Encapsulation** — ATM simulator with PIN + balance protection
5. **Abstraction** — car dashboard simulator, abstract base classes
6. **Inheritance** — vehicle family tree (click any node)
7. **Polymorphism & Method Overriding** — UPI payment + cricket commentator simulators
8. **Composition** — car builder (assemble from engine, wheels, seats, A/C)

### Quiz categories
| Category | Count |
|---|---|
| Basic | 15 |
| Intermediate | 12 |
| Code Output | 13 |
| Interview | 10 |
| **Total** | **50** |

---

## How to Use

```bash
# Clone or download
git clone <repo-url>
cd cs-guide

# Open the hub
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux

# Or open any guide directly
open oops.html
```

No server required. Works 100% offline.

---

## Design System

All guides share the same design tokens and are visually consistent:

- **Color palette** — Indigo primary, purple accent, semantic success/warning/danger
- **Dark mode** — CSS custom properties switched via `body.dark` class
- **Typography** — System font stack, 800-weight headings
- **Components** — Cards, badges, code blocks, output panels, info boxes, simulators
- **Responsive** — CSS Grid with `auto-fit / minmax`, mobile-first breakpoints

---

## Contributing

To add a new topic guide:

1. Create `topic-name.html` following the structure of `oops.html`
2. Add a card in `index.html` inside `.topics-grid` (change badge from "Coming soon" to "Available" and wrap with `<a href="...">`)
3. Update this README

---

Built for learners. Open source. Free forever.
