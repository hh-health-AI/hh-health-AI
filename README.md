<!-- Profile redesign: original graphics and copy; layout inspired by github.com/flycran. -->
<p align="center">
  <img src="./assets/header.svg" width="100%" alt="HH Health AI — healthcare investing, biomedical evidence and AI. Evidence to assumptions to valuation to human judgment." />
</p>

<p align="center">
  <a href="https://github.com/hh-health-AI/healthcare-equity/tree/main/research-suite#quickstart"><b>Try a demo</b></a> &nbsp; · &nbsp;
  <a href="https://github.com/hh-health-AI/healthcare-equity/tree/main/examples/research-cases"><b>Read a research case</b></a> &nbsp; · &nbsp;
  <a href="https://github.com/hh-health-AI/healthcare-equity/tree/main/research-suite/evaluation"><b>Review the evaluation</b></a>
</p>

<blockquote>
  <p align="center"><b>Better evidence. Explicit assumptions. Falsifiable investment views.</b><br />AI should make research more inspectable—not make judgment less accountable.</p>
</blockquote>

## About me

I build open-source tools for **healthcare investing, biotech research and AI-assisted fundamental analysis**. My work connects biomedical evidence and public datasets to the questions that matter for an investment thesis: what changes, how it changes the model, and what would prove the thesis wrong.

- **Research:** Biotech, pharmaceuticals, medtech, life sciences tools and healthcare services.
- **Evidence:** Clinical trials, regulatory catalysts, utilization, reimbursement, provider economics and company filings.
- **Methods:** DCF, risk-adjusted NPV, scenarios, catalyst analysis and evidence-to-valuation workflows.

<!-- geo:start -->
## Start here: Healthcare Equity Research Platform

<table>
<tr><td>
<h3><a href="https://github.com/hh-health-AI/healthcare-equity">healthcare-equity</a></h3>
<p><b>The flagship integration point for healthcare equity research.</b></p>
<p>A synthesis layer and 12 modular evidence pipelines connect clinical and regulatory developments, patient populations, commercial adoption, reimbursement, financial disclosures and valuation.</p>
<p><b>Core value:</b> Turn a source-backed observation into an explicit model assumption and a testable investment view.</p>
<p><code>Clinical evidence</code> → <code>Probability &amp; demand</code> → <code>Commercial assumptions</code> → <code>DCF / rNPV</code> → <code>Investment thesis</code></p>
<p><a href="https://github.com/hh-health-AI/healthcare-equity#monorepo-modules"><b>Explore the modules →</b></a></p>
</td></tr>
</table>

The platform combines **12 evidence modules**, **nine biomedical workflows**, and an investment synthesis layer. Python utilities retrieve data, compare structured records and calculate scenarios; host-loaded skills guide reading and interpretation. The standalone repositories remain authoritative for their specialist scripts; bundled modules are versioned snapshots.
<!-- geo:end -->

## Inspect the research

| Case | Decision question | Reproducible output |
| :--- | :--- | :--- |
| [Biotech: HELIOS-B / vutrisiran](https://github.com/hh-health-AI/healthcare-equity/tree/main/examples/research-cases/biotech-trial-rnpv) | How does clinical evidence differ from a completed approval decision? | Approval-gate and commercial rNPV sensitivities. |
| [Medtech: Intuitive Surgical](https://github.com/hh-health-AI/healthcare-equity/tree/main/examples/research-cases/medtech-procedures-revenue) | How do procedure growth and recurring economics affect revenue? | Platform-specific drivers and revenue sensitivities. |
| [Managed care: medical costs](https://github.com/hh-health-AI/healthcare-equity/tree/main/examples/research-cases/managed-care-mlr-earnings) | What does a medical-cost-ratio change imply for earnings? | Reconciled premiums and static earnings/EPS sensitivities. |

These are dated research demonstrations using real primary-source facts and explicit modeling assumptions. They are not current stock recommendations or fully underwritten price targets.

[Source-backed semantic development set](https://github.com/hh-health-AI/healthcare-equity/tree/main/research-suite/evaluation/semantic) · [Case verification ledger](https://github.com/hh-health-AI/healthcare-equity/blob/main/skills/model-valuation/references/case-source-audit.md) · [Choose an installation path](https://github.com/hh-health-AI/healthcare-equity#installation)

## Research workflow

```mermaid
flowchart TD
    Q["Research question"] --> E["Primary evidence and source ledger"]
    E --> A["Assumptions and uncertainty"]
    A --> M["Models and sensitivities"]
    E --> C["Source and accuracy checks"]
    C --> M
    M --> T["Thesis, catalyst and falsifier"]
    T --> R["Monitor and re-underwrite"]
    R --> E
```

[Detailed source workflow](https://github.com/hh-health-AI/healthcare-equity#workflow) · [Maintenance and synchronization](https://github.com/hh-health-AI/healthcare-equity/blob/main/docs/MAINTENANCE.md)


## Selected research projects

<table>
<tr>
<td width="50%" valign="top">
<h3><a href="https://github.com/hh-health-AI/clinical-catalysts">Clinical catalysts</a></h3>
<p><b>From trial results to underwriting assumptions.</b></p>
<p>Organize trial readouts and regulatory events around approval probability, label, timing and clinical differentiation.</p>
<p><code>Clinical trials</code> <code>FDA catalysts</code></p>
<p><a href="https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/clinical-catalysts">Integrated module →</a></p>
</td>
<td width="50%" valign="top">
<h3><a href="https://github.com/hh-health-AI/cms-reimbursement">CMS reimbursement</a></h3>
<p><b>Understand the economics of market access.</b></p>
<p>Connect coverage and payment evidence to access, pricing assumptions and healthcare business economics.</p>
<p><code>Coverage</code> <code>Payment</code> <code>Market access</code></p>
<p><a href="https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/cms-reimbursement">Integrated module →</a></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<h3><a href="https://github.com/hh-health-AI/rx-utilization">Prescription utilization</a></h3>
<p><b>Test demand against observable evidence.</b></p>
<p>Use prescribing, utilization and launch proxies to challenge commercial assumptions and revenue trajectories.</p>
<p><code>Utilization</code> <code>Launch tracking</code></p>
<p><a href="https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/rx-utilization">Integrated module →</a></p>
</td>
<td width="50%" valign="top">
<h3><a href="https://github.com/hh-health-AI/sec-forensics">SEC forensics</a></h3>
<p><b>Bring financial discipline to the healthcare thesis.</b></p>
<p>Examine company filings, accounting signals and insider activity alongside the scientific and commercial evidence.</p>
<p><code>SEC EDGAR</code> <code>Financial forensics</code></p>
<p><a href="https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/sec-forensics">Integrated module →</a></p>
</td>
</tr>
</table>

<details>
<summary><b>Explore all 12 evidence modules</b></summary>

| Research layer | Integrated module |
| :--- | :--- |
| Clinical and regulatory | [clinical-catalysts](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/clinical-catalysts) |
| Publications, guidelines and expert signals | [evidence-catalysts](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/evidence-catalysts) |
| Safety signals | [fda-safety-signals](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/fda-safety-signals) |
| Prescription utilization | [rx-utilization](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/rx-utilization) |
| Epidemiology and patient populations | [epi-demand](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/epi-demand) |
| Coverage and reimbursement | [cms-reimbursement](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/cms-reimbursement) |
| Provider adoption | [provider-adoption](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/provider-adoption) |
| Provider economics | [provider-economics](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/provider-economics) |
| Procedure and coding exposure | [procedure-exposure](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/procedure-exposure) |
| Patents, exclusivity and loss of exclusivity | [ip-exclusivity](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/ip-exclusivity) |
| International access | [global-access](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/global-access) |
| Company filings and accounting | [sec-forensics](https://github.com/hh-health-AI/healthcare-equity/tree/main/modules/sec-forensics) |

</details>

## Tools and research craft

<p align="center">
  <img src="./assets/toolkit.svg" width="100%" alt="Python for public-data tooling; Markdown for agent instructions; Git for versioned research; GitHub for open collaboration." />
</p>

**Domain expertise:** `Biotech` · `Pharma` · `Medtech` · `Life Sciences Tools` · `Managed Care` · `Healthcare Services` · `Digital Health`

**Research methods:** `DCF` · `rNPV` · `Scenario Analysis` · `Catalyst Research` · `Evidence Synthesis`

<!-- institutional-positioning:start -->
## Research principles

**Primary sources first.** Important numbers should retain their source, vintage and limitations.

**Evidence is not the conclusion.** Observations, assumptions, calculations and investment judgment should remain distinguishable.

**Models must be challengeable.** A thesis needs explicit sensitivities, disconfirming evidence and a clear account of what would change the view.

**Human judgment stays in the loop.** These AI agents, skills and research workflows are designed to support institutional-quality due diligence—not to replace analyst accountability or imply independent certification.
<!-- institutional-positioning:end -->

## Connect

Working on healthcare investing, biomedical data or AI-enabled research? Project issues and pull requests are welcome.

<p align="center">
  <a href="https://github.com/hh-health-AI/healthcare-equity/issues"><b>Contribute a case, adapter or reproducible failure</b></a>
</p>

---

<p align="center"><sub>Research and educational tools—not medical advice or investment recommendations.<br />Public project capabilities vary; inspect each repository's documentation and limitations.</sub></p>
