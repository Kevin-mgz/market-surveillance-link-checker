# AI Usage Transparency

This project was built in collaboration with [Claude](https://claude.ai) (Anthropic), a large language model. This file documents what was human-driven and what was AI-assisted, in the interest of transparency.

---

## What I contributed

- **Process analysis** — identifying the inefficiency in the existing manual workflow and breaking it down into automatable steps
- **Functional specifications** — defining exactly what the tool needed to do : which search combinations to generate, deduplication logic, CSV output format, and data privacy requirements
- **Risk assessment** — evaluating data handling implications (local execution, no external data transmission) to ensure the tool was safe to use in a professional compliance context
- **Testing & validation** — running the tool , verifying the output matched operational needs
- **Project decisions** — scoping what to build now vs. what to defer (e.g. the internal account lookup phase, pending IT API access)

## What AI contributed

- Writing all HTML, CSS, and JavaScript code based on my specifications
- Suggesting the deduplication mechanism for recurring clients across multiple transactions

---

## Why I'm being transparent about this

While my background is not in software development, I have been using code since more than five years. I was able to read through the entire codebase, understand the logic, and validate that the implementation matched the requirements.

I'm transparent about this because it's the honest way to present how modern technical work gets done. Using AI effectively still requires knowing what to build, being able to evaluate what gets produced, and catching what doesn't work. That's what I did here.

---

## Tools used

- **Claude (Anthropic)** — code generation, documentation
- **Browser** — local testing and validation
