
# VIBE Permissive License

The **VIBE License** is a modern permissive open-source license designed for
projects that involve **LLM-generated or LLM-assisted code**. It is inspired by
MIT/BSD, remains short and permissive, and adds:

- A clear **LLM provenance requirement** for modified versions  
- A concise **LLM-generated content disclaimer**
- An optional **LLM Generation Summary** header for transparency
- Full interoperability with modern development workflows

This repository hosts the canonical text of the license and related tools:
README, badges, SPDX identifiers, a CLA, examples, and best practices.

---

## Why the VIBE License Exists

Large Language Models (LLMs) can generate code that:
- may be partially derivative of training data,
- may carry unknown IP risks,
- may lack clear provenance.

Traditional open-source licenses do not address **LLM-generated code** at all.
The VIBE License introduces:

### Transparent provenance  
Contributors must declare which models assisted their updates.

### Modern realism  
It acknowledges that LLMs may reproduce copyrighted or proprietary patterns.

### Permissive simplicity  
The license stays as easy to adopt as MIT/BSD.

### Safety for maintainers  
Maintainers are protected by a no-warranty, no-IP-responsibility clause.

---

## Who Should Use the VIBE License?

Use VIBE if your project includes:

- AI-assisted code  
- LLM-generated modules  
- AI-transformed content  
- Mixed hand-written + LLM-assisted code  
- Educational or experimental AI codebases  
- Tools, libraries, or frameworks that want documented provenance

---

## Provenance Format

For original or modified versions, include:

```
LLM Generation Summary
  - Primary LLM Vendor: OpenAI
  - Primary Model: GPT-5.1
  - Model Version / Date: 2025-12
  - Additional Models (optional):
```

In modified versions, contributors must document:

```
[File or Function Changed]
  - LLM Vendor:
  - Model Name:
  - Model Version:
```

These may be added as:
- code comments
- commit messages
- LICENSE appendices

---

## SPDX Identifier

Use the following in source files:

```
SPDX-License-Identifier: VIBE-1.0
```

---

## Contributor License Agreement (CLA)

This repo includes a `CLA.md` describing:
- contributor rights
- provenance responsibilities
- warranty disclaimers
- licensing terms

Projects MAY optionally require contributors to digitally agree to it.

---

## How to Use the VIBE License in Your Project

1. Copy `LICENSE` into your repository.  
2. Add this header to each source file (optional but recommended):

```
SPDX-License-Identifier: VIBE-1.0
```

3. Add LLM provenance comments when using AI assistance.
4. Ask contributors to accept the CLA (optional, recommended).
5. Add the VIBE badge to your README (TBD)

---

## Example Projects Using VIBE

You may list projects adopting VIBE after publication.

---

## FAQ

### Does VIBE restrict commercial use?  
**No.** It is fully permissive like MIT/BSD.

### Does it require disclosing prompts?  
**No.** Optional only.

### Does it forbid using certain LLMs?  
**No.**

### Is VIBE GPL-compatible?  
Yes. The provenance requirement behaves like MITs attribution.

### Is provenance required for all modifications?  
Only for **LLM-assisted** changes.

---

## License

See `LICENSE` for the full text of the VIBE Permissive License.
