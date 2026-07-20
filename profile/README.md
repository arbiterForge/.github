<div align="center">

<img src="https://raw.githubusercontent.com/arbiterForge/.github/main/profile/AFhero.png" alt="arbiterForge — Where the gate is the only door." width="100%">

<br/><br/>

<b>We build developer tooling where the gate is enforced, not suggested.</b>
<br/>
Intent goes in. A gate-verified PR comes out. Every time.

</div>

---

## The thesis

One rule runs through everything here: no code reaches a branch without clearing the same gated
pipeline, and the proof is never forgeable. We build that rule at two depths.

<div align="center">

<img src="https://raw.githubusercontent.com/arbiterForge/.github/main/profile/gatedPipeline.png" alt="Plain-language intent flows into the gated pipeline (spec, failing tests, commit gate) and out as a gate-verified PR. codeArbiter proves the gate at prompt level; arbiterIDE makes it unforgeable in code." width="100%">

</div>

## Projects

### codeArbiter

<div>

[![Claude Code plugin](https://img.shields.io/badge/Claude_Code-plugin-d97757)](https://github.com/arbiterForge/codeArbiter)
[![Codex plugin](https://img.shields.io/badge/OpenAI_Codex-plugin-10a37f)](https://github.com/arbiterForge/codeArbiter)
[![release](https://img.shields.io/github/v/release/arbiterForge/codeArbiter?label=release)](https://github.com/arbiterForge/codeArbiter/releases)
[![license](https://img.shields.io/github/license/arbiterForge/codeArbiter)](https://github.com/arbiterForge/codeArbiter/blob/main/LICENSE)
[![stars](https://img.shields.io/github/stars/arbiterForge/codeArbiter)](https://github.com/arbiterForge/codeArbiter/stargazers)

</div>

A governance layer for [Claude Code](https://claude.com/claude-code) and OpenAI Codex that refuses
to freelance. Every intent routes through a host-native command to a gated skill or reviewer agent.
Nothing commits until the gates are green, architectural forks are scored through SMARTS instead of
guessed at, and the audit trail (`overrides.log`, ADRs, the sprint log) is append-only and
mechanically guarded. It proves the workflow at prompt level, inside the session, for both hosts
from one shared policy core.

```
/plugin marketplace add arbiterForge/codeArbiter
/plugin install ca@codearbiter
```

Requires Python 3 on `PATH`. Dormant in every repo until you run `/ca:init`, and it writes only to
`.codearbiter/`. See [arbiterForge/codeArbiter](https://github.com/arbiterForge/codeArbiter).

### arbiterIDE

<div>

![status](https://img.shields.io/badge/status-pre--alpha-c0392b)
![platform](https://img.shields.io/badge/platform-Eclipse_Theia-4a6bdc)
![license](https://img.shields.io/badge/license-PolyForm_Noncommercial-8957e5)
![visibility](https://img.shields.io/badge/repo-private-lightgrey)

</div>

Proving the workflow at prompt level has a ceiling. A gate that lives in a transcript is skippable
by a sufficiently creative session, and evidence written as a marker file can be forged.
arbiterIDE moves the structure into code. Gates become interceptors at a single tool-dispatch
chokepoint. Evidence becomes unforgeable HMAC tokens bound to content hashes. The commit path
becomes the only commit path, and CI independently re-derives the verdict server-side, so even a
hostile client cannot fake one.

Built on Eclipse Theia, shipped desktop-first as a branded Electron app. Early and pre-alpha by
design: the full build plan lives in a governed `.codearbiter/` state store the IDE reads and
writes itself, and the repo names what's still scaffolded rather than implying it's all wired.
Private for now. See [arbiterForge/arbiterIDE](https://github.com/arbiterForge/arbiterIDE).

## License

The two projects are licensed differently — check before you build on either. codeArbiter is
[AGPLv3](https://github.com/arbiterForge/codeArbiter/blob/main/LICENSE); network use of a modified
version obligates you to offer that version's source. arbiterIDE is
[PolyForm Noncommercial 1.0.0](https://github.com/arbiterForge/arbiterIDE/blob/main/LICENSE): free
for personal and noncommercial use, with commercial rights reserved. Both hold open a path to a
separate commercial license — ask in an issue on the relevant repo.

## Contact

Open an issue on [codeArbiter](https://github.com/arbiterForge/codeArbiter/issues) or
[arbiterIDE](https://github.com/arbiterForge/arbiterIDE/issues), or start a conversation in
[Discussions](https://github.com/orgs/arbiterForge/discussions).
