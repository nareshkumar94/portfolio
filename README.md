# Naresh.dev — Developer Portfolio

[![Deploy](https://img.shields.io/badge/Deploy-Cloudflare_Pages-F38020?style=flat&logo=cloudflarepages&logoColor=white)](#)
[![Stack](https://img.shields.io/badge/Stack-ES6+_%7C_Tailwind_CDN-06B6D4?style=flat&logo=tailwindcss&logoColor=white)](#)

> Source code for the personal portfolio of **Nareshkumar (Naresh)** — Python Backend & GenAI Developer. Built with zero-dependency vanilla web standards to showcase enterprise ETL pipelines, vectorless RAG, and autonomous AI workflows.

[Explore Live Portfolio →](#)

---

## ⚡ Application Architecture

This website is engineered as a clean, high-performance static Single Page Application (SPA) with zero external build dependencies:

* **Zero-Dependency Static Runtime:** Built with semantic HTML5, modern vanilla JavaScript (ES6+), and CDN-delivered Tailwind CSS. Requires zero compilation or bundling overhead, achieving sub-150ms first-contentful paint globally.
* **Dual-Hydration Pattern:** 
  * In production (HTTP/S), the UI dynamically hydrates from `portfolio-data.json`.
  * For local file inspection (`file:///`) or network constraints, an embedded inline fallback immediately renders all project cards, metrics, and credentials with zero CORS errors.
* **Interactive Telemetry Engine:** In-browser monospace terminal component simulating real structured production log streams (`INFO`, `WARN`, `OK`, `DONE`) across agent decision loops, schema-drift recoveries, and AST retrieval.
* **Obsidian / Amber Theme:** Terminal-inspired dark interface using Obsidian Dark (`#0a0c10`), Terminal Slate (`#12161f`), and Amber Gold accents (`#ec9c13`) with Space Grotesk and Fira Code typography.

---

## 📁 Repository Structure

```text
portfolio/
├── index.html            # Core single-page application (dual-hydrated, responsive)
├── portfolio-data.json   # Single source of truth content model
├── Nareshkumar_Resume.pdf# Current executive resume (PDF)
├── _headers              # Edge CDN cache-control specification (Cloudflare Pages)
└── README.md             # Project documentation
```

---

## 🚀 Running Locally

Because the application implements dual-hydration, it can be tested immediately with zero setup:

### Option 1: Direct File Launch (Offline)
Double-click `index.html` in your file explorer, or run:
```bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
```

### Option 2: Local HTTP Server
```bash
python -m http.server 8000
# Open http://localhost:8000
```
