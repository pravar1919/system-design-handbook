# Contributing to the System Design Handbook

Thank you for helping build a resource that engineers everywhere can learn from. This guide explains how to contribute content that fits the handbook's quality bar.

## Guiding principles

1. **Self-contained chapters.** Every file must stand on its own. A reader landing on your page from a Google search should never need to have read another chapter first. Define acronyms on first use. Don't write "as we discussed earlier."
2. **Teach from first principles.** Motivate every concept with the problem it solves *before* explaining the solution.
3. **Be honest about tradeoffs.** A chapter that only lists advantages is incomplete. The Disadvantages and Tradeoffs sections are mandatory.
4. **Production-grounded.** Prefer concrete numbers, real systems, and named companies over vague generalities. Cite your sources.
5. **Accessible.** Every diagram needs a short text explanation beside it.

## How to add or edit a chapter

1. **Pick a topic** from the [README table of contents](README.md) that is marked 🚧, or open an issue proposing a new one.
2. **Copy [`TEMPLATE.md`](TEMPLATE.md)** into the correct numbered directory.
3. **Name the file** in `kebab-case.md` describing the topic, e.g. `consistent-hashing.md`.
4. **Fill in every section** of the template. Do not leave placeholder sections.
5. **Update the README** status table and, if you added a new chapter, link it in the table of contents.
6. **Open a pull request.** Keep PRs focused — one chapter (or one cohesive edit) per PR.

## Style guide

- **Headings:** Use sentence case (`## The problem this solves`, not `## The Problem This Solves`).
- **Diagrams:** Provide ASCII for simple structures (renders everywhere). Use Mermaid for flows, sequences, and entity relationships. Always caption diagrams.
- **Code:** Use fenced blocks with a language tag. Keep snippets minimal and runnable in spirit.
- **Tone:** Write like a senior engineer explaining to a sharp colleague — clear, direct, no fluff, no marketing.
- **Difficulty badge:** Be realistic. When in doubt, label it one level easier and explain more.
- **Reading time:** Estimate ~200 words/minute of prose, plus ~1 minute per diagram or code block.
- **References:** Link primary sources (papers, official docs, engineering blogs) over secondary summaries.

## What makes a chapter "done"

A chapter is ready to merge when:

- [ ] Every template section is filled with real content.
- [ ] It is self-contained — no unexplained dependencies on other chapters.
- [ ] At least one ASCII and one Mermaid diagram (where the topic warrants visuals).
- [ ] At least two real production examples with citations.
- [ ] Advantages, disadvantages, and tradeoffs are all present and honest.
- [ ] At least 3 interview questions and 2 misconceptions.
- [ ] References point to authoritative sources.
- [ ] Mermaid diagrams render correctly (check on GitHub's preview).

## License

By contributing, you agree that your contributions are licensed under the [CC BY-SA 4.0](LICENSE) license that covers this repository.
