
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

LLMs are increasingly used to generate non-trivial code. While most output follows common, non-protectable patterns, contributors cannot verify the
origin of model output. Traditional OSS licenses do not address this reality.

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

##  When Should You Use the VIBE License?

VIBE was designed for projects where LLM-generated code forms a non-trivial part of the work and where contributors cannot realistically verify the originality of the output. It is most appropriate when the model is helping generate:

- complex logic or workflows
- unusual system designs
- API or architectural patterns with many degrees of creative freedom
- domain-specific implementations
- code where SSO (structure/sequence/organization) may matter
- any content that could plausibly reflect training data

For *simple or conventional boilerplate* (CRUD APIs, React components, standard scripts, common templates), the risk of unique or protectable structure being reproduced is extremely low. In those cases, a traditional permissive license like MIT or BSD is usually sufficient.

VIBE should be viewed as a lightweight, transparent option for situations where *authors cannot confirm originality* and *users deserve clarity*, not as a default for every piece of AI-assisted code.

---

## Provenance Format

For original or modified versions, include:

```
LLM Generation Summary
  - Primary LLM Vendor:
  - Primary Model:
  - Model Version / Date:
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

## Contributor Declarations (Optional Good Practice)

For substantial contributions or releases that involve LLM-generated code,
contributors are encouraged (but not required) to create a `DECLARATION` file
in the repository. This file records:

- the date of the contribution  
- the plagiarism or similarity-check tool used  
- the tool version and scan date  
- a brief statement that no significant similarity was found

This is not a warranty or certification of originality. It is simply a
transparent, timestamped record that a reasonable check was performed.

The VIBE License remains fully permissive regardless of whether this
declaration is included.

---

## Responsible Checks & Reporting

Although LLM-generated code is usually based on common and non-protectable
patterns, users and contributors may choose to run optional code-similarity or
plagiarism checks (e.g., Dolos, CopyLeaks, or similar tools) before releasing
significant modifications. These tools can help detect obvious or accidental
reuse of copyrighted code.

Running such checks is entirely optional and not required by the VIBE License.
Their purpose is to encourage transparency and responsible use, not to certify
originality.


The VIBE License remains fully permissive regardless of whether these checks are
performed.

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

## Why was the VIBE License created?
Existing open-source licenses were written before code could be generated by large language models (LLMs). VIBE adds minimal transparency requirements and realistic disclaimers for projects that use LLM-assisted code, while staying close to MIT/BSD in spirit.

## Does this license restrict commercial or private use?
No. VIBE is fully permissive. Users may run, modify, redistribute, sell, and sublicense the software without limitation.

## What is the provenance requirement?
If a contributor uses an LLM to produce or modify code, they must record:
- LLM vendor  
- model name  
- model version or date  

This can be placed in a commit message, code comment, or appended to the LICENSE file.

## Why is provenance important?
LLM output may have uncertain origins. Provenance:
- informs downstream users,  
- shows the contributor acted in good faith, and  
- avoids implying that the code was hand-written or guaranteed original.

## Does VIBE claim LLM output is dangerous?
No. Most LLM output is based on common patterns that are not protectable by copyright. VIBE simply acknowledges that contributors cannot verify originality.

## Does the license protect me (the author)?
Yes. VIBE includes explicit disclaimers stating:
- authors cannot guarantee originality,
- authors take no responsibility for the IP status of model output,
- downstream users must do their own due diligence.

## Am I liable if the LLM accidentally reproduced copyrighted material?
Possibly. Under most copyright regimes, the party who *distributes* infringing material is liable even without intent. Provenance and realistic disclaimers demonstrate good faith, but do not eliminate legal responsibility.

## Should I keep the prompts used to generate the code?
It is recommended. Prompts:
- show your intent,
- demonstrate you asked for generic or functional output,
- help you in any dispute about willfulness or intent.

## Is SSO (structure/sequence/organization) really copyrightable?
Sometimes. Most common patterns are not protected. But unique, creative, or unusual structures can be. Courts have found SSO infringement in modern cases involving APIs, CLIs, and system architecture.

## Is VIBE GPL-compatible?
Yes in practice. VIBE’s provenance requirement is similar to attribution/NOTICE clauses, which are typically treated as non-restrictive. But it has not been formally tested.

## Can I dual-license my project under VIBE and MIT or Apache?
Yes. Many projects dual-license when introducing new terms. VIBE was intentionally written to be compatible with the permissive license family.

# Legal Appendix

This appendix explains the reasoning behind the provisions of the VIBE License.
It is not part of the license and has no legal force; it is provided for clarity.

## 1. Why disclaim originality?
LLM-generated code may be influenced by patterns in training data.
Contributors cannot realistically trace the origin of generated text or code.
The license therefore makes it explicit that authors provide no guarantee of originality.

## 2. Why assign responsibility to downstream users?
Under copyright law, the party who distributes a work is responsible for the act of distribution.
This applies even if the distributor did not intend to infringe.
The license reflects that reality and does not shift responsibility away from the end user.

## 3. Why require provenance?
Provenance serves two functions:
- It informs downstream users about LLM involvement.
- It documents the contributor's good-faith effort and intent.

Provenance does not guarantee non-infringement. It simply increases transparency.

## 4. SSO (Structure, Sequence, Organization)
Courts have held that the structure or arrangement of a program may be protected
when it reflects creative choices rather than engineering necessity.
Examples include:
- API hierarchy structures
- CLI command organization
- Highly individualized workflows

Most modern patterns are not protectable because they are standard practice.

## 5. Why prompts do not eliminate liability
Prompts are evidence of intent, not proof of originality.
They may mitigate damages in disputes, but they cannot function as a legal shield.

## 6. Why LLM creators are not automatically liable for user distribution
An LLM provider may be responsible for training-related infringement,
but the user is responsible for distributing the output.
These are treated as separate acts under copyright doctrine.

## 7. Why VIBE remains permissive
All additions (provenance, disclaimers) are informational, not restrictive.
They do not impose behavioral restrictions on use, redistribution, or modification.
This maintains compatibility with MIT/BSD-style licensing norms.

---

## License

See `LICENSE` for the full text of the VIBE Permissive License.
