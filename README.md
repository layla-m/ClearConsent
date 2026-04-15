# ClearConsent — Interactive Privacy Consent Interface

> **SOEN 357 · Concordia University**  
> Fawaz Audu (40239173) · Layla Michel (40227408)

---

## Overview

ClearConsent is a cross-platform interactive privacy consent interface designed to improve user comprehension and perceived trust compared to traditional text-based privacy policies. Rather than presenting users with dense legal documents, ClearConsent restructures the consent experience using layered disclosures, visual data representations, and contextual explanations, all embedded naturally within a website's onboarding flow.

ClearConsent is designed to be embedded into existing applications during onboarding, rather than used as a standalone tool.

The prototype demonstrates ClearConsent embedded within **Vitalis**, a simulated health and wellness web application, where ClearConsent appears as Step 3 of a 4-step onboarding process.

---

## Demo

▶️ [Watch the onboarding demo](https://drive.google.com/file/d/1wZdtlRcL4vxOxeLfUUT0WjvKtr113Cli/view?usp=sharing)

---

## Features

**Vitalis Onboarding Flow (4 steps)**
- **Step 1 — Create Account:** Email/password registration with real-time password validation (minimum 8 characters + at least one number or symbol) and per-field error highlighting.
- **Step 2 — Your Profile:** First name, last name, date of birth, and health goal selection with field-specific error feedback.
- **Step 3 — Privacy (ClearConsent):** The full interactive privacy module (see below).
- **Step 4 — All Set:** Success screen with a consent confirmation.

**ClearConsent Privacy Module (Step 3)**
- **High-Level Summary tab:** At-a-glance chips indicating data practices (no selling, deletion rights, third-party partners, optional location, retention period).
- **Data Collected tab:** Expandable cards for each data category (account info, health data, device/usage data, location) with plain-language explanations.
- **Why & How tab:** Purpose panels for each data use case with scenario-based clarifications.
- **Your Rights tab:** Visual cards outlining user rights with one-click access details.
- **Consent tab:** Final review with a live-generated consent stamp, a full data flow diagram, and acceptance controls.
- Progressive disclosure — each tab reveals more detail, reducing cognitive load.
- Functional modals for Terms of Service and the ClearConsent™ information overlay.

**UI / UX Details**
- Dual-brand design system: Vitalis blue (`#0a6ebf`) and ClearConsent green (`#2d6a4f`) via CSS custom properties.
- Live progress bar and step badge that update across all steps and sub-tabs.
- Fully responsive, single-file implementation. No build tools or dependencies required.

---

## Design Rationale

ClearConsent is based on key HCI principles and prior research:
- **Progressive disclosure** to reduce cognitive load (Sweller, 1988)
- **Visual representation** to improve comprehension (Bateman et al., 2010)
- **User control and transparency** to increase trust (Schaub et al., 2015)

---

## Getting Started

No installation needed. Open the file directly in any modern browser:

```bash
open index.html
```

Or drag and drop `index.html` into a browser window.

---

## Project Structure

```
index.html   # Complete prototype (HTML, CSS, and JS in one file)
README.md           # This file
Soen357_ClearConsent_Final_Report.pdf  # Full research paper
```

---

## Research Summary

This project investigates whether an interactive privacy consent interface can measurably improve user understanding and trust. Two interface conditions are compared in a between-subjects experiment:

- **Control:** Traditional scrollable privacy policy with a single acceptance checkbox.
- **Experimental:** ClearConsent's structured, interactive interface.

User comprehension is assessed via multiple-choice questions; trust and usability are measured using Likert-scale surveys and the System Usability Scale (SUS). Cognitive load is evaluated using a rating scale grounded in cognitive load theory.

We hypothesize that participants using ClearConsent will achieve higher comprehension scores, report greater transparency and trust, demonstrate higher usability ratings, and experience lower perceived cognitive load.
