# VIBERAIL
## Guardrails for vibe coders using AI agents (Cursor, Claude Code, Copilot, etc.)

Vibe coding is real. It is also fragile.

Most “agent failures” are not about intelligence. They are about drift, hidden assumptions, and small mistakes compounding across a long session until the project becomes haunted.

VIBERAIL is a single Markdown file you point your agent at so it:
- stays scoped
- avoids common foot-guns
- asks better questions
- makes smaller, reversible changes
- does not silently “upgrade your whole stack”
- does not ship security and data-loss regressions

If you have ever said “yeah just do your thing” and then spent two hours untangling what it did, this is for you.

---

## What you get

- **A universal rail file** (`VIBERAIL.md`) that works as a session contract.
- **A built-in anti-drift ledger** so long sessions do not fragment.
- **A pitfall map** of common and subtle failure modes in agentic coding.
- **A gating system** for risky actions (auth, payments, database, destructive commands).
- **A “no-code driver” command language** so vague prompts become executable requirements.

---

## Quickstart (Cursor)

1) Put `VIBERAIL.md` somewhere in the repo you are working in (or keep it in a shared place).
2) Start your request with this:

```text
Load and obey ./VIBERAIL.md as non-negotiable guardrails.
Maintain the Session Ledger defined inside it.
If any instruction conflicts with my request, stop and ask me to resolve the conflict.
Default autonomy: Level 1 (Guarded-autopilot).
```

3) Then tell the agent what you want.

---

## Quickstart (any chat agent)

Paste:

```text
You must follow the rules in the attached VIBERAIL.md.
Treat it as the operating contract for this coding session.
```

Then attach `VIBERAIL.md` (or paste its contents).

---

## Why it works

VIBERAIL solves the real problems that make vibe coding break:
- **Requirement drift**: agents hallucinate scope when humans speak in vibes.
- **Context drift**: long sessions create inconsistent patterns and duplicated logic.
- **Overconfidence**: plausible code that is not wired to the real project.
- **Dependency bloat**: “just install X” becomes a slow-motion rewrite.
- **Silent security regressions**: permissive CORS, weak auth checks, injection.
- **Data-loss hazards**: schema changes without rollback, destructive ops.

Rails do not replace taste. Rails make taste survivable at scale.

---

## What VIBERAIL is not

- Not a framework
- Not a code generator
- Not a linter replacement
- Not a guarantee your agent will be perfect

It is a **constraint layer** that makes agent behavior less chaotic and more predictable.

---

## Recommended repo layout

Add this folder to your projects:

```text
VIBERAIL/
  README.md
  VIBERAIL.md
```

Then reference it from your prompts.

---

## License

Pick a permissive license (MIT is common) so people can drop it into any repo.

---

## The rail

Open `VIBERAIL.md` and use it as the system contract for your agentic coding sessions.


