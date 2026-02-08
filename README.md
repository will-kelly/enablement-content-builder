# Enablement Content Builder (Custom GPT)

A purpose-built Custom GPT for creating, refining, and standardizing enablement content—optimized for **structured, reusable, audience-appropriate** outputs (training, onboarding, playbooks, internal docs, prompts, and polished drafts).

---

## What it does

Enablement Content Builder helps teams produce clear, consistent enablement materials quickly by:

* Drafting and improving **training / onboarding content**
* Producing **internal documentation and playbooks**
* Generating **enablement prompts and structured guidance**
* Delivering **polished drafts aligned to predefined standards**
* Maintaining a **professional, reusable** tone designed for internal libraries

---

## How it works

This GPT follows a **guided, rules-driven workflow** (an **intake-and-runner** model):

1. **Intake**: Gathers the minimum necessary context (audience, goal, format, tone, constraints).
2. **Runner**: Routes the request into the right content pattern (drafting, rewriting, standardizing, selecting a template, etc.).
3. **Output**: Produces enablement-ready content with consistent structure and formatting.

It’s intentionally *not* a general-purpose chatbot—its focus is enablement workflows and repeatable outputs.

---

## Design principles

### Structured & intent-aware

* Uses a routing model instead of improvising
* Optimized for “make me a usable artifact” outcomes

### Consistent tone and formatting

* Professional, clear, and reusable for internal audiences

### Prompt-library aligned

* Prefers established patterns/templates instead of inventing new frameworks

### Outcome-focused

* Minimizes extra explanation and gets to usable deliverables fast

---

## What it avoids

* Free-form creativity without structure (unless explicitly requested)
* Off-scope assistance (personal advice, entertainment, unrelated general chat)
* Inventing new frameworks when established patterns exist
* Assuming missing context (uses intake flow instead of guessing)

---

## Repository contents

Typical files used to define and operate this GPT:

* `gpt.json` — GPT identity/config and core behavior
* `intake_and_runner.json` — the intake + routing workflow definition
* `prompt_library.json` — reusable prompt patterns and standardized templates

---

## Getting started

### Option A: Use in ChatGPT (Custom GPT)

1. Open ChatGPT → **Explore GPTs** → **Create**
2. Configure the GPT using the contents of:

   * `gpt.json`
   * `intake_and_runner.json`
   * `prompt_library.json`
3. Save and publish privately (recommended) or to your workspace

### Option B: Use as a source-controlled definition

* Store the JSON files in this repo
* Review changes via PRs for governance (tone, templates, routing rules)
* Tag releases when prompt patterns or standards change

---

## Usage examples (copy/paste)

### 1) Create a playbook

> Create a sales discovery playbook for SMB reps. Audience: new hires. Include sections: goals, qualification, talk tracks, pitfalls, checklist.

### 2) Standardize an existing doc

> Here’s a rough onboarding doc. Rewrite to match our enablement standard: scannable headings, step-by-step, role-based callouts, and a final checklist.

### 3) Generate training content

> Build a 30-minute training module for “Handling pricing objections.” Include facilitator notes, slides outline, and a role-play exercise.

### 4) Produce reusable prompts

> Create a reusable prompt template for drafting internal product launch enablement updates.

---

## Contributing

Contributions should preserve the GPT’s enablement-first behavior:

* Add or refine templates in `prompt_library.json` (prefer patterns over one-offs)
* Update intake questions only when they reduce ambiguity or improve routing
* Keep outputs consistent: scannable structure, clear sections, minimal fluff

Suggested PR checklist:

* [ ] Does this improve reuse across teams?
* [ ] Does it reduce ambiguity without adding unnecessary steps?
* [ ] Does it preserve the standardized tone/format?
* [ ] Did you add examples or update templates where needed?

---

## License

Add your preferred license (e.g., MIT / Apache-2.0 / proprietary internal). If this is internal enablement IP, consider a private repo with restricted access.

---

