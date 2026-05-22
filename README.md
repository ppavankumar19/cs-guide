# CS Guide — Interactive Computer Science Learning

A collection of interactive guides to core Computer Science concepts. No frameworks, no build tools, no installation — just open an HTML file in any browser and start learning.

**Live site:** https://ppavankumar19.github.io/cs-guide/

---

## Project Structure

```
cs-guide/
├── index.html                  ← Hub page — topic selection
├── oops.html                   ← Object-Oriented Programming guide (complete)
├── backend-mastery.html        ← Backend Mastery guide (complete)
├── fundamentals-mastery.html   ← Fundamentals Mastery guide (complete)
└── README.md                   ← You are here
```

---

## Topics

| Topic | Link | Status |
|---|---|---|
| Object-Oriented Programming | `oops.html` | ✅ Available |
| Data Structures & Algorithms | [aikaryashala.com/gvpcew](https://aikaryashala.com/gvpcew/index.html) | ✅ Available (external) |
| Backend Mastery | `backend-mastery.html` | ✅ Available |
| Fundamentals Mastery | `fundamentals-mastery.html` | ✅ Available |
| Computer Networks | — | 🔜 Coming soon |
| Operating Systems | — | 🔜 Coming soon |
| Database Management | — | 🔜 Coming soon |
| System Design | — | 🔜 Coming soon |
| Python Fundamentals | — | 🔜 Coming soon |

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
- **Back to top button** — floating scroll-to-top on all pages
- **Home button** — nav link back to `index.html` on all topic pages

---

## Fundamentals Mastery Guide — What's Covered (`fundamentals-mastery.html`)

6 topics, 9 live simulators, 60 quiz questions, ~90 min read time:

1. **Route vs Routing** — what a route is, static vs dynamic routes, path params vs query params, client-side vs server-side routing, file-based routing
2. **File Handling (C & Python)** — open/read/write/append/close, C vs Python side-by-side, file cursor visualizer, context managers vs manual fclose
3. **Variable Scope** — LEGB rule, local vs global vs enclosing, `global` and `nonlocal` keywords, interactive scope explorer
4. **Database Indexing** — full table scan vs B-Tree lookup, index types, composite indexes, when to/not to index, Index Race simulator
5. **Pick a Database** — SQLite vs MySQL vs PostgreSQL: embedded vs client-server, concurrency, features, when to use each, DB Recommender simulator
6. **SQL Queries** — SELECT, WHERE, ORDER BY, LIMIT, INSERT, UPDATE, DELETE, aggregate functions, GROUP BY, HAVING, JOINs (INNER/LEFT/RIGHT/FULL OUTER), JOIN Visualizer simulator

### Simulators
| Simulator | Topic |
|---|---|
| URL Navigator — live route matching | Routing |
| Client vs Server routing visualizer | Routing |
| C vs Python language switcher | File Handling |
| File Operations Playground (read/write/append) | File Handling |
| File Cursor Visualizer (seek/readline) | File Handling |
| Scope Explorer — click any line | Variable Scope |
| Index Race — full scan vs B-Tree | Database Indexing |
| DB Recommender — 4-question picker | Pick a Database |
| JOIN Visualizer — INNER/LEFT/RIGHT/FULL | SQL Queries |

### Quiz categories
| Category | Count |
|---|---|
| Routing | 10 |
| Files | 10 |
| Scope | 10 |
| Indexing | 10 |
| Databases | 10 |
| Queries | 10 |
| **Total** | **60** |

---

## Backend Mastery Guide — What's Covered (`backend-mastery.html`)

6 topics, 8 live simulators, 50 quiz questions, ~90 min read time:

0. **What is an API?** — Intro & foundation: what APIs are, why they exist, how a request/response cycle works
1. **CORS** — Same-origin policy, preflight requests, `Access-Control-Allow-Origin`, browser vs server perspective
2. **Middleware** — Request/response pipeline, logging, auth, rate limiting, error handlers in Express & FastAPI
3. **REST API** — HTTP methods, status codes, resource design, statelessness, REST constraints
4. **FastAPI** — Route builder, Pydantic validation, dependency injection, async endpoints
5. **SOAP API** — XML envelope structure, WSDL, fault handling, REST vs SOAP comparison

### Quiz categories
| Category | Count |
|---|---|
| CORS | 10 |
| Middleware | 10 |
| REST | 10 |
| FastAPI | 10 |
| SOAP | 10 |
| **Total** | **50** |

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
# Clone
git clone https://github.com/ppavankumar19/cs-guide.git
cd cs-guide

# Open the hub
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

No server required. Works 100% offline.

---

## Design System

All guides share the same design tokens:

- **Color palette** — Indigo primary, purple accent, semantic success/warning/danger
- **Dark mode** — CSS custom properties switched via `body.dark` class
- **Typography** — System font stack, 800-weight headings
- **Components** — Cards, badges, code blocks, output panels, info boxes, simulators
- **Responsive** — CSS Grid with `auto-fit / minmax`, mobile-first breakpoints

---

## Contributing

To add a new topic guide:

1. Create `topic-name.html` following the structure of `oops.html`
2. Add a card in `index.html` inside `.topics-grid` with class `available` and an `<a href="...">` wrapper
3. Update the Topics table in this README

For external guides, link directly from the card using `target="_blank" rel="noopener noreferrer"`.

---

Built for learners. Open source. Free forever.
