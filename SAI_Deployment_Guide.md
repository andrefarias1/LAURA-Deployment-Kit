# SAI Deployment Guide
## How to Deploy LAURA at Your Supreme Audit Institution

> **Audience:** SAI administrators, IT teams, and audit methodology leaders responsible for deploying and configuring LAURA.

---

## 1. Overview

LAURA (Logical Audit Understanding & Review Assistant) is an AI-powered audit assistant that guides auditors through the complete audit lifecycle — from planning through execution and reporting. It is built on INTOSAI standards (ISSAI 100, 300, 3000, 400, 4000) and can be adapted to any SAI's specific methodology, templates, and legal framework.

### What's in the Kit

```
LAURA-Deployment-Kit/
├── README.md                              ← You are here (start here)
├── LAURA_Core_Instructions.md             ← The AI system prompt
├── knowledge-base/
│   ├── ISSAI_Core_Reference.md            ← INTOSAI standards synthesis
│   ├── Audit_Methodology_Reference.md     ← Generic audit methods
│   └── Findings_Reporting_Framework.md    ← Findings, reporting, proposals
└── SAI_Deployment_Guide.md                ← This guide
```

### How LAURA Works

LAURA operates in two layers:

1. **Core Layer (provided in this kit):** INTOSAI-aligned standards, generic audit methodology, and the complete P0–P7 / E0–E8 workflow. This is the "engine" that works out of the box for any SAI.

2. **SAI Layer (provided by you):** Your SAI's specific audit manual, standards, report templates, recommendation framework, and legal basis. This layer makes LAURA produce outputs that conform to your institutional requirements.

The more SAI-specific documents you provide, the more tailored LAURA's outputs become. Without them, LAURA still works — but outputs follow generic INTOSAI conventions.

---

## 2. Platform Deployment

LAURA is platform-agnostic. The instructions and knowledge base files work on any AI platform that supports system prompts and document uploads. Here are deployment instructions for the most common platforms:

### 2.1 Claude (Anthropic) — Projects

1. Create a new **Claude Project** at claude.ai.
2. In the Project's **System Prompt**, paste the entire contents of `LAURA_Core_Instructions.md`.
3. Upload the three knowledge base files to the project's **Knowledge** section:
   - `ISSAI_Core_Reference.md`
   - `Audit_Methodology_Reference.md`
   - `Findings_Reporting_Framework.md`
4. Upload your SAI-specific documents (see Section 3) to the same Knowledge section.
5. Start a conversation — LAURA will activate.

### 2.2 ChatGPT (OpenAI) — Custom GPT

1. Go to **Create a GPT** at chat.openai.com.
2. In **Instructions**, paste the entire contents of `LAURA_Core_Instructions.md`.
3. Upload the three knowledge base files under **Knowledge**:
   - `ISSAI_Core_Reference.md`
   - `Audit_Methodology_Reference.md`
   - `Findings_Reporting_Framework.md`
4. Upload your SAI-specific documents to the same Knowledge section.
5. Optionally enable **Code Interpreter** (for data analysis) and **Web Browsing** (for research).
6. Save and publish (privately or to your organisation).

### 2.3 Other Platforms (Microsoft Copilot Studio, Google AI Studio, Open-Source LLMs)

The general pattern is the same:
1. Insert `LAURA_Core_Instructions.md` as the system prompt / instruction set.
2. Attach the knowledge base files as reference documents or retrieval sources.
3. Attach your SAI-specific documents.
4. Configure the model to prioritise attached documents over general knowledge.

> **Tip:** If your platform has a token/context limit, prioritise your SAI-specific documents over the LAURA Core knowledge base files. The AI model's general training already covers much of the INTOSAI content; your SAI-specific documents are what make LAURA truly useful.

---

## 3. Preparing Your SAI-Specific Documents

### 3.1 Required Documents (R1–R5)

These documents are essential for LAURA to produce SAI-compliant outputs. For each, we describe what LAURA needs and how to prepare it.

#### R1: Audit Manual / Methodology Guide
**What LAURA needs:** The document that defines how audits are conducted at your SAI — phases, steps, deliverables, approval workflows.

**How to prepare:**
- If you have a single comprehensive audit manual, upload it as-is.
- If you have separate manuals for performance and compliance audits, upload both.
- Acceptable formats: PDF, DOCX, Markdown, or plain text.
- If the manual is very large (>100 pages), consider providing a condensed version with the most critical procedural sections.

#### R2: Audit Standards / Norms
**What LAURA needs:** Your SAI's official audit standards — the equivalent of national auditing standards or quality standards that auditors must follow.

**How to prepare:**
- Upload the official document.
- If your SAI directly adopts ISSAI standards without modification, you can note this instead of uploading the full ISSAI texts (LAURA's core knowledge base already covers ISSAI 100/300/3000/400/4000).

#### R3: Report Template or Structure Guide
**What LAURA needs:** The official format for audit reports — required sections, their order, formatting rules, style guidelines.

**How to prepare:**
- A template document showing the expected structure (even with placeholder content) is ideal.
- Alternatively, a style guide describing the required sections and formatting rules.
- If possible, include a sample completed report (see O5).

#### R4: Recommendations / Determinations Framework
**What LAURA needs:** The rules for how your SAI formulates proposals — types of proposals (recommendations, determinations, orders, etc.), language requirements, categorisation criteria, deadline rules, legal basis.

**How to prepare:**
- This may be a standalone regulation, a chapter of your audit manual, or an internal directive.
- Key information LAURA needs:
  - What types of proposals does your SAI issue? (e.g., recommendations, determinations, orders)
  - What are the language requirements for each type? (imperative? subjunctive?)
  - Must each proposal address a single issue?
  - Are deadlines required for certain types?
  - What is the legal basis for each type?

#### R5: Legal / Institutional Framework Summary
**What LAURA needs:** The key laws and regulations that govern your SAI's mandate, authority, and operations.

**How to prepare:**
- A summary document is sufficient — LAURA does not need the full text of every law.
- Include: the SAI's enabling legislation, key regulations on audit procedures, relevant constitutional provisions, any special laws affecting audit scope or authority.
- Focus on provisions that affect how audits are conducted and reported.

### 3.2 Optional Documents (O1–O10)

These enhance LAURA's effectiveness but are not required:

| Doc | What to Prepare |
|-----|----------------|
| **O1** Risk Framework | Your SAI's risk assessment methodology or policy |
| **O2** QA Procedures | Quality assurance standards, checklists, review procedures |
| **O3** Internal Control Guide | How your SAI evaluates auditee internal controls |
| **O4** Findings Matrix Template | Your SAI's specific template for documenting findings |
| **O5** Sample Reports | 1–3 past audit reports (anonymised if needed) for LAURA to learn tone and structure |
| **O6** Audit Design Matrix Template | Your SAI's specific planning matrix format |
| **O7** Code of Ethics | Your SAI's ethical standards |
| **O8** Glossary | SAI-specific terminology definitions |
| **O9** Concessions/PPPs Reference | If relevant to your SAI's mandate |
| **O10** Sector-Specific Guides | Methodology for specific sectors |

### 3.3 Document Preparation Tips

- **Format:** Markdown (.md) or plain text (.txt) produces the best results with AI systems. PDF and DOCX also work but may have formatting issues.
- **Size:** Most AI platforms have limits on how much reference material they can process. If your documents are very large, consider:
  - Extracting the most relevant chapters/sections.
  - Creating a condensed version focusing on procedures, templates, and rules.
  - Prioritising R1–R5 over optional documents if space is limited.
- **Language:** LAURA Core instructions are in English. If your SAI's documents are in another language, LAURA can still process them — it will read them in the original language and produce outputs in the language you specify. However, you may also translate or summarise your key documents into English for better accuracy.
- **Anonymisation:** If uploading sample reports, anonymise any sensitive information (names of auditees, confidential findings, etc.).

---

## 4. First-Time Configuration Walkthrough

After deploying LAURA on your chosen platform with the core files and your SAI documents, the first interaction will trigger the **Onboarding Protocol**:

1. **LAURA greets the user** and presents the Required Documents Checklist.
2. **The user confirms** which documents have been uploaded (or uploads them in the conversation).
3. **LAURA processes the documents** and builds an SAI Profile — a summary of your SAI's key parameters.
4. **The user validates** the SAI Profile (terminology mapping, report structure, proposal rules).
5. **LAURA is ready** — the audit workflow begins.

> **Tip:** Run the onboarding with your methodology team first. Validate the SAI Profile carefully — it determines how LAURA will behave for all subsequent interactions.

---

## 5. Customisation Options

### 5.1 Terminology Overrides
If your SAI uses different terms for standard concepts, ensure they are captured in your documents or explicitly tell LAURA during onboarding. For example:
- "At our SAI, we call the Audit Design Matrix a 'Work Programme'"
- "We use 'Observations' instead of 'Findings'"
- "Our proposals are called 'Orders' (mandatory) and 'Advisories' (optional)"

### 5.2 Workflow Modifications
The P0–P7 / E0–E8 workflow is designed to be comprehensive. Your SAI may:
- **Merge steps:** Some SAIs combine risk assessment (P3) with the design matrix (P4). Tell LAURA.
- **Skip steps:** E4 (Accountability Matrix) is already optional. Other steps may be skippable for certain audit types.
- **Add steps:** If your SAI has additional steps (e.g., a mandatory peer review step), describe them in your audit manual (R1) and LAURA will incorporate them.

### 5.3 Output Format Preferences
LAURA supports three output formats:
- **DOCX** (Word) — Best for editable reports and formal deliverables
- **PDF** — Best for final, non-editable versions
- **Markdown** — Best for technical users and version control

Specify your preference during onboarding or at any step.

### 5.4 Language
LAURA Core is in English, but LAURA can produce outputs in any language. To set the language:
- Include documents in your preferred language.
- Tell LAURA: "Please produce all outputs in [language]."
- LAURA will adapt its output language while maintaining the same structure and methodology.

---

## 6. Maintenance and Updates

### 6.1 Updating SAI Documents
When your SAI updates its audit manual, standards, or templates:
1. Prepare the updated document (following the guidelines in Section 3).
2. Replace the old version in your deployment platform's knowledge base.
3. Inform LAURA in a new conversation: "Our audit manual has been updated. Please re-read and update the SAI Profile."

### 6.2 Updating LAURA Core
When a new version of LAURA Core is released:
1. Replace `LAURA_Core_Instructions.md` with the new version.
2. Replace the knowledge base files with their new versions.
3. Your SAI-specific documents remain unchanged.
4. Test with a quick interaction to ensure compatibility.

### 6.3 Feedback Loop
Encourage auditors to provide feedback on LAURA's outputs:
- Are the templates accurate?
- Is the terminology correct?
- Are there steps or deliverables that LAURA misses?
- Are there additional SAI documents that should be uploaded?

Use this feedback to refine your SAI-specific documents and improve LAURA's accuracy over time.

---

## 7. Troubleshooting

| Issue | Solution |
|-------|----------|
| LAURA uses wrong terminology | Check the SAI Profile. Provide explicit terminology corrections during the conversation or update your documents. |
| Outputs don't match SAI templates | Upload a more detailed template document (R3, O4, O6). Include examples. |
| LAURA skips a step | Ask LAURA to go back: "Please take me to step P3." LAURA supports navigation. |
| Outputs are too generic | Upload more SAI-specific documents. The more context LAURA has, the more tailored its outputs. |
| LAURA can't read a document | Convert to Markdown or plain text. PDF with images (scanned documents) may not be readable. |
| Platform token limit exceeded | Reduce document sizes. Prioritise R1–R5 over optional documents. Use condensed versions. |
| LAURA produces outputs in the wrong language | Explicitly state the desired output language: "All outputs should be in French." |

---

## 8. Security Considerations

- **Do not upload** classified or top-secret documents to commercial AI platforms.
- **Anonymise** sensitive information in sample reports before uploading.
- **Verify** your AI platform's data privacy and retention policies.
- LAURA's system instructions include protections against prompt injection and instruction extraction. However, the AI platform's overall security posture should be evaluated by your IT team.
- For SAIs with strict data sovereignty requirements, consider deploying LAURA on a self-hosted AI infrastructure using open-source models.

---

## 9. Quick-Start Checklist

Use this checklist to deploy LAURA in under 30 minutes:

- [ ] **Choose a platform** (Claude Projects, Custom GPT, or other)
- [ ] **Paste** `LAURA_Core_Instructions.md` as the system prompt
- [ ] **Upload** the three knowledge base files
- [ ] **Prepare** at least documents R1–R3 (audit manual, standards, report template)
- [ ] **Upload** your SAI-specific documents
- [ ] **Start a conversation** — LAURA will initiate onboarding
- [ ] **Validate** the SAI Profile LAURA generates
- [ ] **Test** with a simple audit scenario (e.g., "Start a new performance audit of programme X")
- [ ] **Refine** — add more SAI documents based on initial experience
- [ ] **Roll out** to your audit teams

---

*SAI Deployment Guide v1.0 — LAURA Deployment Kit*
