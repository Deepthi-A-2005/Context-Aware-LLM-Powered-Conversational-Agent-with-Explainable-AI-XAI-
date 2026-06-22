# Context-Aware-LLM-Powered-Conversational-Agent-with-Explainable-AI
# NeuralContext XAI — Frontend Prototype

A multi-screen UI prototype for an **Explainable AI (XAI) platform** with real-time model transparency, RAG configuration, and MLOps dashboards.

## 📁 Project Structure

```
neuralcontext/
├── index.html                          # Navigation hub
├── neuralcontext-landing-page.html     # Public marketing landing page
├── xai-interactive-dashboard.html     # Main XAI explainability dashboard
├── xai-assistant-conversational-intelligence.html  # Chat + reasoning trace
├── performance-metrics.html           # Live metrics & evaluation charts
├── model-and-rag-configuration.html   # Model selection & RAG pipeline config
├── context-and-memory-management.html # Context window & memory management
├── deployment-and-mlops-dashboard.html # CI/CD, deployment health, MLOps
├── technical-architecture.html        # System architecture diagrams
├── technical-implementation-and-api-docs.html # API reference docs
│
├── css/
│   └── shared.css                     # Design tokens, components, dark mode
│
├── js/
│   └── shared.js                      # Chart utils, dark mode, animations
│
└── README.md
```

## 🚀 Key Features

- **Dark / Light mode** — persisted via `localStorage`, respects system preference
- **Shared design system** — CSS custom properties for consistent theming
- **Real canvas-rendered charts** — Line, bar, and donut charts (no external chart lib needed)
- **Interactive attention heatmaps** — Token-level attention weight visualization
- **Animated metrics** — Numbers count up on page load / scroll-into-view
- **Responsive layout** — Collapsible sidebar on mobile, fluid grids
- **Accessible** — Focus-visible rings, ARIA labels, reduced-motion support

## 🎨 Design System

### Color Palette
| Token | Light | Dark |
|-------|-------|------|
| `--color-primary` | `#49607e` | `#b0c8eb` |
| `--color-secondary` | `#00677e` | `#3cd7ff` |
| `--color-accent-vivid` | `#00d2fd` | `#00d2fd` |
| `--color-surface` | `#f7fafd` | `#181c1e` |

### Typography
- **Display / Headline**: Inter (700–800)
- **Body**: Inter (400–600)
- **Code / Labels / Mono**: JetBrains Mono

## 🛠 Tech Stack

- **Tailwind CSS v3** (CDN) — utility classes
- **Material Symbols Outlined** — icon font
- **Inter + JetBrains Mono** — Google Fonts
- **Vanilla JS + Canvas 2D API** — charts, animations, dark mode

## 📊 Screens

| Screen | Purpose |
|--------|---------|
| Landing Page | Public-facing hero, feature overview, CTA |
| XAI Dashboard | Attention maps, token attribution, logic chains |
| Conversational Intelligence | Chat UI with live reasoning trace panel |
| Performance Metrics | Accuracy/latency charts, human eval table |
| Model & RAG Config | Model picker, retrieval settings, chunk config |
| Context & Memory | Context window timeline, memory slot manager |
| Deployment & MLOps | Canary deploys, service health, CD pipelines |
| Technical Architecture | System topology diagram, data flow |
| API Docs | Endpoint reference, code samples, auth guide |

## 🔧 Local Development

No build step required. Open `index.html` in any modern browser:

```bash
# Using Python's built-in server (recommended for font loading)
python3 -m http.server 8080
# Then open http://localhost:8080
```

Or use VS Code Live Server / any static file server.

## 📄 Google Interview Notes

This project demonstrates:
- **Component thinking** — shared CSS/JS modules, reusable card/button/badge system
- **Data visualization** — custom Canvas 2D charts (no library dependency)
- **Accessibility** — semantic HTML, focus management, ARIA, reduced motion
- **Performance** — IntersectionObserver for lazy chart rendering, CSS transitions over JS
- **Dark mode** — CSS custom properties pattern, theme persistence
- **Responsive design** — mobile-first grid system, collapsible navigation
