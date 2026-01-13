# ECISA — Executive Continuity & Institutional Stability Act

![ECISA banner](ECISA_banner.png)

**Model Act and implementation scaffolding for continuity floors and capacity-aware guardrails on high-impact executive actions.**

> If an executive action is big enough to disable essential functions or wipe out operational capacity, it must pass through a short, enforceable public process: publish impacts, define continuity floors, and accept rapid independent review.

---

## 1. What ECISA is (and why it exists)

Modern government can be broken faster than elections, courts, or Congress can respond.

One coordinated wave of:

- mass firings or coerced resignations,
- mass “reclassification” that strips due-process protections,
- or abrupt shutdown / transfer of load-bearing programs

can collapse essential services long before any oversight body sees the real numbers.

ECISA (Executive Continuity & Institutional Stability Act) is a **model statute** designed to stop that specific failure mode:

- It **does not** freeze agencies in place.
- It **does not** block lawful discipline for cause.
- It **does** make it very hard to quietly gut capacity in the dark.

In plain terms, ECISA says:

- You can change policy.  
- You can reform agencies.  
- You can discipline people **for cause**.  
- But you **cannot** quietly switch off load-bearing functions or wipe out essential capacity without:
  - defining what is essential,
  - publishing what will break and by how much,
  - and giving independent oversight offices a fast chance to review.

This repository packages:

- The **model act text** (bill-drafting ready).  
- **Minimum templates** for:
  - Essential Function Registers (EFRs) — where agencies define Essential Functions and Continuity Floors.  
  - Continuity Impact Statements (CIS) — what must be published before high-impact actions take effect.  
- A **plain-language companion explainer** for legislators, staff, oversight bodies, and journalists.

The goal: give legislators, counsel, and governance engineers a **copy-paste-ready legislative core** plus enough scaffolding to implement it in the real world.

### For legislators, staff, and oversight offices

If you’re here to understand or brief ECISA, start with:

- `docs/ECISA_Companion_Explainer_v1.0.md`  
  Plain-language explainer for policymakers, legislative counsel, IG/GAO/OPM staff, and journalists.

If you need the binding text and implementation surfaces:

- `docs/ECISA_Model_Act_v0.1.md`  
- `docs/ECISA_CIS_Template_v1.0.md`  
- `docs/ECISA_EFR_Template_v1.0.md`

Those three are the **canonical design surface** of this repo.

---

## 2. What ECISA does and does not do

ECISA **does**:

- Require each agency to define **Essential Functions** and publish **Continuity Floors**.  
- Force high-impact actions (mass staffing reductions, large-scale reclassification, elimination or transfer of Essential Functions) through a **Continuity Impact Statement (CIS)**.  
- Require a **fast, public Review Note** from IG / GAO / OPM (or equivalents) before such actions take effect.  
- Provide a **time-limited emergency derogation** path with 72-hour publication and sunset.  

ECISA **does not**:

- Freeze agencies in place or forbid reforms.  
- Block lawful discipline for cause or Congressionally mandated budget cuts.  
- Choose vendors, software systems, or specific implementation technologies.  
- Make the President “weak” — it makes capacity destruction **expensive in daylight**, not impossible.

Think of ECISA as a **continuity standard** for institutions, not a partisan weapon:
it protects whoever wins the next election from inheriting a hollowed-out state.

---

## 3. Core mechanic (threat model in one page)

ECISA targets a narrow but dangerous failure mode: **abrupt capacity destruction** that disables Essential Functions faster than Congress, courts, or elections can respond.

Mechanically, it works by:

1. **Essential Function Register (EFR)**  
   Each agency publishes an EFR listing Essential Functions, baseline capacity metrics, and **Continuity Floors** — the minimum staffing/authority needed to avoid systemic harm.

2. **High-Impact Action trigger**  
   If an executive action is big enough to:
   - cut workforce by a large percentage in a short window, or  
   - eliminate/suspend an Essential Function, or  
   - reclassify or migrate Essential Functions at scale,  

   it is classified as a **High-Impact Action** and triggers a CIS.

3. **Continuity Impact Statement (CIS)**  
   Before the action takes effect (except in narrow emergencies), the initiating authority must publish a CIS describing:
   - what is being done and under what legal authority,  
   - which Essential Functions are affected and by how much,  
   - expected service and risk impacts,  
   - alternatives considered and rollback triggers.

4. **Independent Review Note**  
   IG / GAO / OPM (or equivalents) issue a brief **Review Note**:
   - they do **not** approve policy;  
   - they certify completeness, auditability, and non-evasion of due process.

5. **Emergency derogation**  
   If delay would cause imminent harm, action can begin immediately, but:
   - a short-form CIS must be published within 72 hours; and  
   - emergency authority sunsets unless regular ECISA process catches up.

---

## 4. How a Hill office or oversight team would actually use this

In practice, a Hill office, IG team, or GAO unit could use ECISA as a **checklist**:

1. **Ask for the EFR**  
   - “Show us your Essential Function Register and Continuity Floors.”
2. **Ask for the CIS**  
   - “For this mass staffing / reclassification / shutdown: where is the Continuity Impact Statement?”
3. **Ask for the Review Notes**  
   - “Where are the IG / GAO / OPM Review Notes, with timestamps?”
4. **Compare against outcomes**  
   - “Did metrics land where the CIS said they would, or is there unreported damage?”

The statute creates the **obligation**; the templates make it **easy to see** when someone is trying to dodge it.

---

## 5. Repository structure

Minimal v0.1 layout:

- `docs/ECISA_Model_Act_v0.1.md`  
  **Normative text.** Full model statute suitable for bill drafting, adaptation, and legislative counsel review.

- `docs/ECISA_Companion_Explainer_v1.0.md`  
  **Non-normative explainer.** Plain-language overview for legislators, staff, oversight offices, and journalists.

- `docs/ECISA_CIS_Template_v1.0.md`  
  **Non-normative template.** Minimum required fields for a Continuity Impact Statement (CIS).

- `docs/ECISA_EFR_Template_v1.0.md`  
  **Non-normative template.** Minimum required fields for an Essential Function Register (EFR).

- `meta/HASHES.md`  
  SHA-256 hashes for the canonical core docs (model act + implementation templates), to support integrity anchoring.

- `meta/NOTARIZATION.md`  
  Notes and placeholders for external timestamping / notarization (e.g., OpenTimestamps).

- `LICENSE`  
  License terms (non-derivative, attribution-required, non-commercial resale without separate license) aligned with the SPARK-NITT governance stack.

(Additional briefs or notes may be added under `docs/` over time; unless explicitly stated, they are **non-normative** companions, not changes to the Model Act.)

---

## 6. Integrity and hashing

In keeping with the rest of the SPARK-NITT governance stack, this repository treats **the model act and implementation templates** as the canonical core.

Only the following files are included in `meta/HASHES.md`:

- `docs/ECISA_Model_Act_v0.1.md`  
- `docs/ECISA_CIS_Template_v1.0.md`  
- `docs/ECISA_EFR_Template_v1.0.md`  

The `README.md` and non-normative explainers (including `ECISA_Companion_Explainer_v1.0.md`) are **not** hashed, so they can be refined for clarity and accessibility without forcing a rehash of the standard.

You may additionally anchor `meta/HASHES.md` itself via external timestamping (e.g., OpenTimestamps) and record receipts in `meta/NOTARIZATION.md`.

---

## 7. License

This repository is intended to be licensed under a **non-derivative, attribution-required license** consistent with the SPARK-NITT governance stack (for example, a “no-derivatives, no commercial resale without separate license” posture).

In effect:

- You may redistribute the text **only as an unchanged copy**, with clear attribution to the author (`SPARK-NITT`).  
- Any derivative legislative drafting, commentary, or tooling should state clearly where it diverges.  
- Commercial use or integration into paid products requires a separate license from the author.

See the `LICENSE` file for the operative terms.

---

## 8. Status and non-advice disclaimer

- Version: **v0.1** (Model Act draft for public comment and legislative adaptation).  
- Audience: legislators, legislative counsel, governance engineers, civil servants, journalists, and researchers.

This repository:

- is **not legal advice**;  
- does **not** create an attorney-client relationship;  
- does **not** bind any jurisdiction or actor.

Any attempt to introduce ECISA (or a derivative) as legislation must go through standard democratic, legal, and professional review channels in the relevant jurisdiction.
