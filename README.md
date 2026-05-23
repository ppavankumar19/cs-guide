# CS Guide — Interactive Computer Science Learning

A collection of interactive guides and coding assessments for core Computer Science concepts. No frameworks, no build tools, no installation — just open an HTML file in any browser and start learning.

**Live site:** https://ppavankumar19.github.io/cs-guide/

---

## Project Structure

```
cs-guide/
├── index.html                      ← Hub page — topic selection + assessments tab
├── oops.html                       ← Object-Oriented Programming guide
├── backend-mastery.html            ← Backend Mastery guide (CORS, REST, FastAPI, SOAP)
├── fundamentals-mastery.html       ← Fundamentals Mastery guide (SQL, Files, Scope…)
├── assessment-python-oops-api.html ← Coding assessment: Python + OOPS + APIs
├── assessment-sql.html             ← Coding assessment: SQL (MySQL / PostgreSQL / SQLite3)
└── README.md                       ← You are here
```

---

## Guides

| Topic | File | Status |
|---|---|---|
| Object-Oriented Programming | `oops.html` | ✅ Available |
| Data Structures & Algorithms | [aikaryashala.com/gvpcew](https://aikaryashala.com/gvpcew/index.html) | ✅ Available (external) |
| Backend Mastery | `backend-mastery.html` | ✅ Available |
| Fundamentals Mastery | `fundamentals-mastery.html` | ✅ Available |
| Computer Networks | — | 🔜 Coming soon |
| Operating Systems | — | 🔜 Coming soon |
| System Design | — | 🔜 Coming soon |

---

## Assessments

| Assessment | File | Questions | Duration |
|---|---|---|---|
| Python · OOPS · APIs | `assessment-python-oops-api.html` | 11 | 1 Hour |
| SQL (MySQL · PostgreSQL · SQLite3) | `assessment-sql.html` | 30 | 1 Hour |

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
- **Scroll progress bar** — top-of-page reading progress indicator
- **Back to top button** — floating scroll-to-top on all pages
- **Home button** — nav link back to `index.html` on all topic pages

---

## Assessments — What's Covered

### Python + OOPS + APIs (`assessment-python-oops-api.html`)

11 questions, 3 sections, 1 hour:

| Section | Topics |
|---|---|
| Section A — Logic Building | Prime numbers, prime factors, recursion (reverse, factorial) |
| Section B — OOPS | Student result system, inheritance, encapsulation, polymorphism |
| Section C — API Programming | FastAPI GET route, POST with Pydantic, HTTP middleware |

### SQL Assessment (`assessment-sql.html`)

30 questions, 6 sections, 1 hour — MySQL / PostgreSQL / SQLite3:

| Section | Topics |
|---|---|
| Section A — SELECT & Filtering | SELECT *, column selection, aliases, DISTINCT, WHERE, AND, IN, LIKE, BETWEEN, IS NULL |
| Section B — Sorting & Pagination | ORDER BY ASC/DESC, LIMIT, OFFSET (pagination) |
| Section C — Aggregate Functions | COUNT, SUM, AVG, MAX, MIN, GROUP BY, HAVING |
| Section D — JOINs | INNER JOIN, LEFT JOIN, finding unmatched rows (NULL check) |
| Section E — Write Operations | INSERT, UPDATE, DELETE |
| Section F — Subquery & Indexing | Subquery with AVG, CREATE INDEX, EXPLAIN / EXPLAIN ANALYZE / EXPLAIN QUERY PLAN |

**Database tables used:** `users`, `orders`, `employees`, `departments`

---

## Fundamentals Mastery Guide (`fundamentals-mastery.html`)

6 topics, 9 live simulators, 60 quiz questions, ~90 min read time:

1. **Route vs Routing** — static vs dynamic routes, path params vs query params, client-side vs server-side routing
2. **File Handling (C & Python)** — open/read/write/append/close, file cursor visualizer
3. **Variable Scope** — LEGB rule, local/global/enclosing, `global` and `nonlocal` keywords
4. **Database Indexing** — full table scan vs B-Tree lookup, index types, composite indexes
5. **Pick a Database** — SQLite vs MySQL vs PostgreSQL, DB Recommender simulator
6. **SQL Queries** — SELECT, WHERE, JOINs, aggregate functions, JOIN Visualizer

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

---

## Backend Mastery Guide (`backend-mastery.html`)

6 topics, 8 live simulators, 50 quiz questions, ~90 min read time:

1. **What is an API?** — request/response cycle, how APIs work
2. **CORS** — same-origin policy, preflight requests, `Access-Control-Allow-Origin`
3. **Middleware** — request/response pipeline, logging, auth, rate limiting
4. **REST API** — HTTP methods, status codes, resource design, statelessness
5. **FastAPI** — route builder, Pydantic validation, dependency injection, async
6. **SOAP API** — XML envelope structure, WSDL, fault handling, REST vs SOAP

---

## OOP Guide (`oops.html`)

8 core concepts, 8 live simulators, 50 quiz questions:

1. **Class & Object** — blueprint vs instance, tea shop simulator
2. **self** — how Python passes the current object to methods
3. **Constructor (`__init__`)** — phone setup phase simulator
4. **Encapsulation** — ATM simulator with PIN + balance protection
5. **Abstraction** — car dashboard simulator, abstract base classes
6. **Inheritance** — vehicle family tree (click any node)
7. **Polymorphism & Method Overriding** — UPI payment + cricket commentator simulators
8. **Composition** — car builder (assemble from engine, wheels, seats, A/C)

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

All pages share the same design tokens:

- **Color palette** — Indigo primary, purple accent, semantic success/warning/danger/info/teal
- **Dark mode** — CSS custom properties switched via `body.dark`, persisted in localStorage
- **Typography** — Plus Jakarta Sans + JetBrains Mono for code blocks
- **Components** — Cards, badges, code blocks, output panels, info boxes, simulators
- **Responsive** — CSS Grid with `auto-fit / minmax`, mobile-first breakpoints at 1024 / 768 / 640 / 600 / 480px
- **Accessibility** — focus-visible outlines, aria-labels, semantic HTML

---

## Contributing

To add a new topic guide:

1. Create `topic-name.html` following the structure of `oops.html`
2. Add a card in `index.html` inside `.topics-grid` with class `available` and an `<a href="...">` wrapper
3. Update the Topics table in this README

To add a new assessment:

1. Create `assessment-topic.html` following the structure of `assessment-sql.html`
2. Add a card in `index.html` inside the Assessments tab's `.topics-grid`
3. Update the Assessments table in this README

For external guides, link directly from the card using `target="_blank" rel="noopener noreferrer"`.

---

Built for learners. Open source. Free forever.
