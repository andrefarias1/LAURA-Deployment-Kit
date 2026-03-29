# Findings & Reporting Framework
## LAURA Core Knowledge Base

> **Purpose:** This document provides LAURA with generic, SAI-agnostic knowledge of how to structure audit findings, build findings matrices, draft audit reports, formulate recommendations/determinations, and handle the accountability process. SAIs should supplement this with their own report templates, recommendation standards, and legal frameworks.

---

## 1. The Findings Matrix

### 1.1 Purpose
The Findings Matrix is the central document of the execution phase. It systematises all audit findings by providing a structured, complete description of each finding and its associated elements. It serves as the foundation for the audit report.

### 1.2 Finding Structure (INTOSAI Standard)
Each audit finding must contain the following core elements:

| Element | Description | Key Question |
|---------|-------------|--------------|
| **Title** | A concise, descriptive label for the finding | What is this about? |
| **Condition / Situation Found** | Factual description of what was observed | What did we find? |
| **Criteria** | The benchmark, standard, law, or regulation that should apply | What should be? |
| **Evidence** | Proof that supports the condition | How do we know? |
| **Cause** | The root reason for the gap between condition and criteria | Why did it happen? |
| **Effect / Consequence** | The impact or risk resulting from the gap | What are the consequences? |
| **Recommendation / Proposed Action** | Suggested corrective or improvement action | What should be done? |
| **Expected Benefit** | The anticipated result of implementing the recommendation | What will improve? |

### 1.3 Findings Matrix Template

```
┌─────────────────────────────────────────────────────────┐
│ FINDINGS MATRIX                                          │
│ Audit: [Audit Title]                                     │
│ Date: [Date]                                             │
├──────┬──────────────────────────────────────────────────┤
│ ID   │ FND-01                                            │
├──────┼──────────────────────────────────────────────────┤
│ Title│ [Concise finding title]                           │
├──────┼──────────────────────────────────────────────────┤
│ Audit│ [Link to audit question QST-XX]                   │
│ Quest│                                                    │
├──────┼──────────────────────────────────────────────────┤
│ Risk │ [Link to mapped risk RIS-XX]                      │
│ Ref  │                                                    │
├──────┼──────────────────────────────────────────────────┤
│ Cond.│ [Objective, factual description of what was       │
│      │  observed during the audit]                        │
├──────┼──────────────────────────────────────────────────┤
│ Crit.│ [Applicable standard, law, regulation, benchmark] │
├──────┼──────────────────────────────────────────────────┤
│ Evid.│ [List of evidence supporting the condition]        │
│      │ EV-001: [description]                              │
│      │ EV-002: [description]                              │
├──────┼──────────────────────────────────────────────────┤
│ Cause│ [Root cause analysis — why the gap exists]         │
├──────┼──────────────────────────────────────────────────┤
│ Eff. │ [Actual or potential consequences — financial,     │
│      │  operational, social, legal]                       │
├──────┼──────────────────────────────────────────────────┤
│ Prop.│ [Recommendation or determination]                  │
│ Actn.│ - Responsible entity: [who should act]             │
│      │ - Deadline: [if applicable]                        │
│      │ - Type: [Recommendation / Determination]           │
├──────┼──────────────────────────────────────────────────┤
│ Benf.│ [Expected financial and/or non-financial benefit]  │
└──────┴──────────────────────────────────────────────────┘
```

### 1.4 Relationship: Risk → Finding
Risks identified during planning (RIS-XX) may become findings (FND-XX) during execution if the audit confirms that the risk has materialised. The Findings Matrix should trace each finding back to the corresponding risk(s) and audit question(s).

### 1.5 Completeness Check
Before finalising the Findings Matrix:
- [ ] Every finding has all core elements (Condition, Criteria, Cause, Effect)
- [ ] Every element is supported by specific evidence
- [ ] Each recommendation logically addresses the identified cause
- [ ] Each recommendation is feasible and within the auditee's competence
- [ ] Cross-references to audit questions and risks are complete
- [ ] No finding is marked as "incomplete" or "[TO BE DEFINED]"

---

## 2. Recommendations and Determinations

### 2.1 Definitions
SAIs typically issue two types of proposals:

- **Recommendation:** A suggestion for improvement. Usually addresses performance gaps, systemic weaknesses, or opportunities to enhance economy, efficiency, or effectiveness. The auditee has discretion in how to implement. Language is typically subjunctive ("The SAI recommends that...").
- **Determination:** A mandatory corrective action. Usually addresses legal non-compliance, irregularities, or situations requiring immediate correction. Language is typically imperative ("The SAI determines that...").

> **Note:** Terminology varies by SAI. Some SAIs use: "orders", "directives", "rulings", "decisions", "requirements", "suggestions". LAURA adapts to the terminology provided in the SAI's configuration documents.

### 2.2 Quality Criteria for Proposals
Every recommendation or determination should be:

| Criterion | Description |
|-----------|-------------|
| **Clear** | Unambiguous; the auditee knows exactly what is expected |
| **Specific** | Addresses a single issue per proposal (avoid bundling) |
| **Feasible** | Implementable within the auditee's capacity and authority |
| **Objective** | Addresses the root cause, not just symptoms |
| **Actionable** | Identifies the responsible entity/agent |
| **Time-bound** | Includes a deadline (especially for determinations) |
| **Beneficial** | States the expected benefit or purpose |
| **Within scope** | Falls within the SAI's mandate and the audit's scope |
| **Properly categorised** | Correctly classified as recommendation or determination |
| **Non-prescriptive** | (For recommendations) Does not dictate the exact method; allows managerial discretion |

### 2.3 Common Proposal Defects
LAURA should flag:
- Proposals that are too generic or vague
- Proposals that bundle multiple issues into one
- Proposals without a clearly identified responsible party
- Determinations without deadlines
- Proposals that exceed the SAI's legal mandate
- Recommendations that impose obligations beyond the auditee's competence
- Language mismatch (imperative language for recommendations, or subjunctive for determinations)
- Proposals that do not address the root cause of the finding

### 2.4 Proposals Checklist Template
For each proposal in the report:

```
□ Addresses a single, specific issue
□ Clearly identifies the responsible entity/agent
□ Correctly categorised (Recommendation / Determination)
□ Deadline specified (if determination)
□ Language matches the category (imperative / subjunctive)
□ Based on a documented finding with supporting evidence
□ Addresses the root cause identified in the finding
□ Is feasible and within the responsible entity's competence
□ States the expected benefit or purpose
□ Falls within the SAI's legal mandate and audit scope
□ Does not impose illegal obligations
□ Is clear and unambiguous
```

---

## 3. Accountability Matrix (Optional)

### 3.1 Purpose
When the audit identifies potential irregularities involving individual responsibility (fraud, gross negligence, wilful misconduct), an Accountability Matrix may be developed. This is separate from the main audit report and supports potential disciplinary, administrative, or judicial proceedings.

> **Note:** Not all audits require an Accountability Matrix. It is typically used when there is evidence of: fraud, overbilling, wilful violation of law, gross negligence causing damage, or other serious misconduct. The decision to develop it should be agreed with the audit supervisor/user.

### 3.2 Accountability Matrix Structure
For each identified irregularity:

| Element | Description |
|---------|-------------|
| **Irregularity** | Description of the unlawful or irregular act |
| **Responsible Party(ies)** | Name, role/position, identification details of persons involved |
| **Conduct** | Description of the action or omission attributed to each responsible party |
| **Causal Link** | How the conduct contributed to or caused the irregularity |
| **Intent / Culpability** | Assessment of intent (wilful) or negligence; consideration of mitigating/aggravating circumstances |
| **Legal Provisions Violated** | Specific laws, regulations, or rules violated |
| **Evidence** | Evidence supporting the irregularity and the attribution of responsibility |
| **Proposed Sanction / Action** | Recommended disciplinary, administrative, or legal action |

### 3.3 Important Considerations
- Use objective, evidence-based language — avoid accusatory adjectives
- Establish clear causal link between the conduct and the irregularity
- Consider whether the responsible party had the duty and the ability to act differently
- Document mitigating circumstances where relevant
- Follow the SAI's internal procedures for handling accountability matters
- Accountability matters are typically handled separately from the public audit report

---

## 4. Audit Report Architecture

### 4.1 Generic Report Structure (INTOSAI-Aligned)
While each SAI has its own report format, most audit reports contain the following sections:

| Section | Content |
|---------|---------|
| **Cover Page** | Audit title, SAI identity, report number, date |
| **Table of Contents** | Structured navigation with page numbers |
| **Executive Summary** | Key findings, conclusions, and recommendations (≤2 pages) |
| **1. Introduction** | Context, legal basis, objective, authorisation |
| **2. Scope and Methodology** | What was audited, time period, methods used, limitations |
| **3. Subject Matter Overview** | Description of the audited entity/programme/activity |
| **4. Audit Findings** | Detailed findings (Condition, Criteria, Cause, Effect) grouped by theme or audit question |
| **5. Conclusion** | Overall assessment responding to the audit objective |
| **6. Recommendations / Proposals** | Numbered list of all recommendations and determinations |
| **7. Auditee Comments** | Summary of the auditee's response to preliminary findings and the audit team's analysis |
| **Annexes** | Findings Matrix, Audit Design Matrix, evidence catalogue, methodology details |

### 4.2 Report Writing Principles
- **Objectivity:** Present facts, not opinions. Let evidence speak.
- **Impersonal voice:** Use third person ("The audit team found..." not "We found...").
- **Clarity:** Write for non-specialists. Define technical terms. Use plain language.
- **Conciseness:** Include only relevant information. Avoid redundancy.
- **Accuracy:** Every statement must be supported by evidence.
- **Completeness:** All significant findings must be reported.
- **Constructiveness:** Focus on improvement, not blame.
- **Balance:** Include positive aspects and good practices where observed.
- **Timeliness:** Reports should be issued within a reasonable timeframe.

### 4.3 Report Sections — Detailed Guidance

#### Executive Summary
- Maximum 2 pages
- Structured: Objective → Key Findings → Main Conclusions → Principal Recommendations
- Should stand alone — a reader should understand the audit from the summary alone
- Written last, after the full report is complete

#### Introduction
- Legal basis for the audit (SAI mandate, authorising decision)
- Audit objective
- Brief context (why this audit, why now)
- Audit team composition (optional, per SAI standards)

#### Scope and Methodology
- What was examined (entities, programmes, time period, geographic scope)
- What was NOT examined (scope limitations)
- Methods used (document review, interviews, data analysis, etc.)
- Sampling approach (if applicable)
- Criteria sources
- Limitations and their impact on conclusions

#### Subject Matter Overview
- Description of the audited entity, programme, or activity
- Legal and institutional framework
- Key stakeholders
- Relevant financial/budgetary information
- Recent history and context
- Should draw from the Subject Matter Overview produced during planning (P2)

#### Audit Findings
- Each finding presented in a structured format
- Grouped logically (by audit question, theme, or significance)
- Include evidence references
- Summarise the finding narrative (full detail goes in the Findings Matrix annex)
- Each finding should include: the situation found, the criteria, the cause, and the effect

#### Conclusion
- Direct response to the audit objective
- Supported by the findings presented
- No new information introduced
- All recommendations/determinations should be at least briefly mentioned
- Forward-looking: what needs to change

#### Recommendations / Proposals
- Numbered sequentially
- Each linked to a specific finding
- Clearly categorised (recommendation vs. determination)
- Include responsible entity and deadline where applicable

#### Auditee Comments
- Present a summary of the auditee's response to the preliminary report
- Analyse the arguments presented
- State whether any findings or recommendations were adjusted as a result
- Maintain a technical, respectful tone
- This section demonstrates due process (adversarial principle)

### 4.4 Logical Consistency Check
Before finalising the report:
- [ ] The conclusion responds directly to the audit objective
- [ ] Every finding in the conclusion appears in the findings section
- [ ] Every recommendation corresponds to a specific finding
- [ ] All recommendations in the conclusion also appear in the proposals section
- [ ] References to annexes (matrices, evidence) are correct
- [ ] Page numbering, headers, and table of contents are accurate
- [ ] No "[TO BE DEFINED]" markers remain in the text
- [ ] Terminology is consistent throughout

---

## 5. The Adversarial Process (Contradictory / Due Process)

### 5.1 Principle
The auditee has the right to know and respond to audit findings before the final report is issued. This:
- Strengthens the accuracy and fairness of the report
- Provides the auditee an opportunity to correct errors or provide additional evidence
- Demonstrates the SAI's commitment to due process
- Enhances the credibility and legitimacy of audit conclusions

### 5.2 Process
1. **Preliminary Report** — Sent to the auditee containing findings and proposed recommendations
2. **Response Period** — The auditee is given a defined period to respond (per SAI standards)
3. **Analysis** — The audit team analyses the auditee's comments
4. **Adjustment** — Findings are adjusted if the auditee provides compelling evidence
5. **Documentation** — The auditee's comments and the team's analysis are included in the final report

### 5.3 Rules
- The preliminary report should NOT include information whose disclosure could compromise audit objectives (e.g., fraud investigations)
- Proposals for sanctions or accountability actions may be excluded from the preliminary version
- The absence of a response from the auditee does not prevent the report from being finalised
- The tone of the audit team's response to auditee comments must be technical and respectful

---

## 6. Report Quality Checklist (Generic)

| # | Quality Criterion | Check |
|---|-------------------|-------|
| 1 | Audit objective is clearly stated | □ |
| 2 | Scope and methodology are adequately described | □ |
| 3 | Subject matter overview is accurate and current | □ |
| 4 | All findings have the required elements (Condition, Criteria, Cause, Effect) | □ |
| 5 | All findings are supported by sufficient, relevant evidence | □ |
| 6 | Conclusions are supported by findings (no new information) | □ |
| 7 | Recommendations address root causes | □ |
| 8 | Recommendations are clear, feasible, and properly categorised | □ |
| 9 | Auditee comments are included and properly addressed | □ |
| 10 | Language is objective, impersonal, and clear | □ |
| 11 | Report structure follows SAI standards | □ |
| 12 | Executive summary accurately reflects the report | □ |
| 13 | All cross-references and annexes are correct | □ |
| 14 | No residual placeholders ("[TO BE DEFINED]") | □ |
| 15 | Formatting is consistent (numbering, headers, fonts) | □ |

---

*Findings & Reporting Framework v1.0 — LAURA Deployment Kit*
*Sources: ISSAI 100/300/3000/400/4000, generic SAI best practices*
