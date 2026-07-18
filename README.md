= Technical Writing Portfolio

This repository demonstrates a *Docs-as-Code* methodology, focusing on automated CI/CD pipelines, structured markup architecture, and scalable documentation infrastructure.

== Documentation Library

=== API & Technical Reference
* <<api-samples/llm-generation-api.adoc#, Chat Completions API>>:: Schema architecture, authentication protocols, and request/response payloads for the v1/chat/completions endpoint.

=== Security & Compliance
* <<asciidoc-samples/sensitive-data-sop.adoc#, SOP: Sensitive Data Sanitization>>:: Security protocols for scrubbing PII and sensitive tokens from logs prior to system audit.

=== Engineering Standards & Guides
* <<markdown-samples/grammarly-guide.adoc#, Grammarly Integration Guide>>:: Configuration and voice-consistency standards for writing assistance tools.
* <<markdown-samples/markdown-formatting-guide.adoc#, Documentation Standards>>:: Structural requirements and formatting conventions for the documentation library.

== Infrastructure
* *Pipeline:* Automated publishing via custom GitHub Actions (`.github/workflows/docs-pipeline.yml`).
* *Deployment:* CI/CD integration with GitHub Pages for static HTML distribution.

== Core Competencies
* *Domains:* API/Webhook documentation, Security Compliance (PII/IAM), and SaaS end-user manuals.
* *Markup:* Proficient in AsciiDoc (Asciidoctor ecosystem) and GitHub Flavored Markdown.
* *Tooling:* Git version control, CI/CD pipeline orchestration, and command-line automation.
