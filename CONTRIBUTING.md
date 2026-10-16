# Contributing to Brierfield Pathway projects

These guidelines apply to active software, documentation tooling, websites and infrastructure code in the **brierfieldpathway** organisation. They supplement, not replace, each repository's current instructions and required safety/release checks.

## Start with the approved requirement

- Before writing functional code in a **new** repository, start from the approved [Brierfield Labs project template](https://github.com/brierfieldlabs/_template) or an equivalent approved organisation-accessible copy, and complete its short `PROJECT.md`. The initial GitHub creation commit is not a functional-code commit.
- Existing repositories should adopt the principles in place, without rewriting their stack or overwriting established project-specific instructions.
- At the start of a session, read the repository's `AGENTS.md` (if present), current README, issue/PR backlog, decisions and applicable house rules. The central [Brierfield Labs Coding House Rules](https://github.com/brierfieldlabs/infrastructure/blob/main/procedures/coding-house-rules.md) are available to authorised contributors.
- Work only on an accepted requirement. Record additional suggestions as **proposed or deferred issues**, not as unrequested implementation.

## Build less, deliver more

- Implement the smallest maintainable, useful change. Reuse what works; don't introduce a new service, framework, database, abstraction or configuration layer merely because it might be useful one day.
- Make security controls proportionate to identified risks. Protect genuine private information, credentials, business data, integrity and recovery needs; neither over-engineer protections nor silently weaken necessary ones.
- Keep tests relevant to changed behaviour and realistic failure modes. Respect established CI, approval and release gates; don't multiply checks or tests for their own sake.
- Keep prior technical decisions unless new evidence or the project owner changes the requirement. Ask before significant scope or architecture expansion.
- Preserve upstream coding conventions, licences and contributor requirements in forks.

## GitHub workflow

1. Link the task to the appropriate GitHub issue (or explain a small maintenance change), work on a branch and open a concise PR.
2. Explain what changed, why this is the simplest sufficient solution, and any genuinely new dependency or risk.
3. Run the repository's established validation on the appropriate environment; don't claim CI or a deployment succeeded without evidence.
4. Keep current documentation aligned with the code. Push work to the canonical GitHub repository and leave a clear next action. Don't strand the only copy of a decision or implementation in chat or on a workstation.
5. Merge and deploy only according to the repository's existing approval and release policy. A green PR isn't automatic permission to publish production changes.

ChatGPT/Codex and other authorised agents follow the same rules. **The goal is useful working software, not maximum code or maximum process.**

Organisation default files provide guidance only. GitHub's repository templates and these defaults do not by themselves technically block non-compliant first commits.
