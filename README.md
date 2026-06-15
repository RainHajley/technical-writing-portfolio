# Docs-as-Code Technical Writing Portfolio

Welcome! This repository serves as a live presentation of modern developer documentation engineering, SaaS training manuals, and enterprise API references. I treat documentation as software—utilizing structured markup languages, clean semantic patterns, and automated CI/CD validation pipelines.

---

## 📂 Portfolio Architecture & Deliverables

This repository is organized into distinct domain folders to demonstrate versatility across varying engineering and corporate requirements:

* **`/api-samples`** (Markdown)
  * **[AI Chat Completions API Reference](./api-samples/llm-generation-api.md)**: A high-level technical reference guide detailing authentication headers, request payloads, model temperature tuning parameters, and JSON token usage objects.

* **`/markdown-samples`** (Markdown)
  * **[How to Use Grammarly in Google Docs](./markdown-samples/grammarly-guide.md)**: An end-user training manual featuring interface navigation, step-by-step onboarding sequences, and visual layout troubleshooting matrixes.
  * **[Markdown Formatting Styling Standards](./markdown-samples/markdown-formatting-guide.md)**: An internal developer guide establishing code block fencing syntax, typographical conventions, and relative linking configurations.

* **`/asciidoc-samples`** (AsciiDoc)
  * **[SOP: Handling Sensitive Client Data](./asciidoc-samples/sensitive-data-sop.adoc)**: A highly structured compliance document showcasing AsciiDoc-specific document attributes, automatic cross-referencing headers, and risk-severity tables.

---

## 🛠️ Automated CI/CD Infrastructure

This workspace utilizes a decoupled publishing pipeline to render and host documents natively:
* **The Engine:** A custom GitHub Actions automated workflow pipeline (`.github/workflows/docs-pipeline.yml`).
* **The Output:** The pipeline compiles raw structured assets and pipes the production static distribution files directly into the `/docs` directory.
* **The Deployment:** GitHub Pages automatically maps and broadcasts live, accessible HTML outputs directly from the `/docs` build folder.

---

## 🧰 Core Competencies
* **Technical Domains:** API & Webhook Specifications, IAM / Security Compliance Systems, SaaS End-User Manuals.
* **Markup Architectures:** Markdown (GFM), AsciiDoc (Asciidoctor Ecosystem).
* **Engineering Toolkit:** Git/GitHub Workflows, GitHub Actions Automation Pipelines, Command-Line Utilities.
