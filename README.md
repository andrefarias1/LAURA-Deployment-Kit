# LAURA Deployment Kit
## Logical Audit Understanding & Review Assistant — For Supreme Audit Institutions

---

### What is LAURA?

LAURA is an AI-powered assistant that guides auditors through the complete audit lifecycle:

```
PLANNING (P0–P7)  →  EXECUTION & REPORTING (E0–E8)
```

It supports **performance audits** (economy, efficiency, effectiveness) and **compliance audits** (conformity with laws and regulations), aligned with **INTOSAI standards** (ISSAI 100, 300, 3000, 400, 4000).

LAURA is designed to be deployed by any Supreme Audit Institution (SAI) worldwide. It ships with a lean, INTOSAI-based core and adapts to each SAI's specific standards, templates, and legal framework through a structured onboarding process.

---

### Architecture

```
┌──────────────────────────────────────────────────────────┐
│                    LAURA RUNTIME                          │
│                                                           │
│  ┌─────────────────────┐   ┌──────────────────────────┐  │
│  │   CORE LAYER         │   │   SAI LAYER               │  │
│  │   (This Kit)         │   │   (Provided by each SAI)  │  │
│  │                      │   │                            │  │
│  │  System Instructions │   │  Audit Manual        (R1) │  │
│  │  ISSAI Reference     │   │  Audit Standards     (R2) │  │
│  │  Methodology Ref     │   │  Report Template     (R3) │  │
│  │  Findings Framework  │   │  Proposals Framework (R4) │  │
│  │                      │   │  Legal Framework     (R5) │  │
│  │                      │   │  + Optional docs  (O1–10) │  │
│  └─────────────────────┘   └──────────────────────────┘  │
│                                                           │
│  Priority: SAI Layer > Core Layer > AI Training Knowledge │
└──────────────────────────────────────────────────────────┘
```

The **Core Layer** provides INTOSAI-aligned methodology that works for any SAI. The **SAI Layer** customises LAURA to your institution's specific requirements. The more SAI documents you provide, the more tailored the outputs.

---

### File Inventory

| File | Description | Size |
|------|-------------|------|
| `README.md` | This file — overview and quick-start | — |
| `LAURA_Core_Instructions.md` | The system prompt — paste into your AI platform | ~12 KB |
| `SAI_Deployment_Guide.md` | Step-by-step deployment and customisation guide | ~10 KB |
| `knowledge-base/ISSAI_Core_Reference.md` | Synthesised ISSAI 100/300/3000/400/4000 standards | ~12 KB |
| `knowledge-base/Audit_Methodology_Reference.md` | Generic audit methods, risk frameworks, data collection | ~12 KB |
| `knowledge-base/Findings_Reporting_Framework.md` | Findings structure, report architecture, proposals | ~12 KB |

**Total Core footprint:** ~58 KB — deliberately lean to maximise space for SAI-specific documents.

---

### Quick Start (5 Minutes)

1. **Choose a platform:** Claude Projects, Custom GPT, or any AI platform with system prompts and document upload.
2. **Paste** the contents of `LAURA_Core_Instructions.md` as the system prompt.
3. **Upload** the three files in `knowledge-base/` as reference documents.
4. **Upload** your SAI-specific documents (at minimum: audit manual, standards, report template).
5. **Start a conversation.** LAURA will guide you through onboarding and begin.

For detailed instructions, see `SAI_Deployment_Guide.md`.

---

### The Audit Workflow

#### Planning Phase (P0–P7)

| Step | What Happens | Output |
|------|-------------|--------|
| P0 | Contextualise the case | Initial Briefing |
| P1 | Define audit strategy | Audit Canvas |
| P2 | Understand the audit object | Subject Matter Overview |
| P3 | Assess risks | Risk Matrix |
| P4 | Design the audit | Audit Design Matrix |
| P5 | Build collection instruments | Work Papers |
| P6 | Consolidate the plan | Audit Plan |
| P7 | Quality review | Quality Checklist + Presentation |

#### Execution & Reporting Phase (E0–E8)

| Step | What Happens | Output |
|------|-------------|--------|
| E0 | Load the approved plan | Planning Extract |
| E1 | Collect evidence | Catalogued Evidence |
| E2 | Analyse evidence | Documented Analyses |
| E3 | Build findings | Findings Matrix |
| E4 | Accountability (optional) | Accountability Matrix |
| E5 | Draft the report | Report Draft |
| E6 | Verify proposals | Proposals Checklist |
| E7 | Review and revise | Revised Report |
| E8 | Export final report | Final Report (DOCX/PDF/MD) |

---

### Standards Foundation

LAURA Core is built on:

| Standard | Coverage |
|----------|----------|
| ISSAI 100 | Fundamental principles of public sector auditing |
| ISSAI 300 / 3000 | Performance audit standards and guidelines |
| ISSAI 400 / 4000 | Compliance audit standards and guidelines |
| COSO ERM (2017) | Enterprise risk management framework (for internal control assessment) |

---

### Supported Output Formats

- **DOCX** — Editable Word documents
- **PDF** — Final formatted reports
- **Markdown** — Plain text with formatting (technical users, version control)

---

### Language Support

LAURA Core instructions are in **English**. However, LAURA can:
- Read SAI documents in **any language**
- Produce outputs in **any language** (just specify during onboarding or at any step)
- Handle multilingual workflows (e.g., read documents in French, produce reports in French)

For SAIs that need the instructions themselves translated, we recommend translating `LAURA_Core_Instructions.md` into your working language before deployment.

---

### Origin

LAURA was originally developed for Brazil's **Tribunal de Contas da União (TCU)** as a specialised audit assistant. This Deployment Kit is the internationalised, SAI-agnostic version — stripped of all TCU-specific content and rebuilt on INTOSAI standards, ready for adoption by any SAI.

---

### Versioning

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2025 | Initial release — Core instructions, 3 knowledge base files, deployment guide |

---

### License and Attribution

This kit is provided for use by Supreme Audit Institutions. When deploying LAURA, please credit:

> LAURA (Logical Audit Understanding & Review Assistant) — originally developed by ANDRE L. A. FARIAS for SAI Brazil, internationalised for the INTOSAI community.

---

*LAURA Deployment Kit v1.0*
