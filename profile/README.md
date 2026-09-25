<div align="center">

<img src="https://raw.githubusercontent.com/arbiterForge/.github/main/profile/AFhero.png" alt="arbiterForge" width="100%">

<br/><br/>

<b>We build developer tooling where the gate is enforced, not suggested.</b>
<br/>
Repository-owned context, explicit decisions, and inspectable development evidence.

</div>

---

## The thesis

codeArbiter brings governed development lanes into supported coding hosts.
arbiterIDE is a separate editor project. Each product owns its implementation,
threat boundary and release evidence; shared intent is not a shared guarantee.

<div align="center">

<img src="https://raw.githubusercontent.com/arbiterForge/.github/main/profile/gatedPipeline.png" alt="Concept illustration of intent, specification, tests, commit review and delivery." width="100%">

</div>

The illustration describes the design direction, not qualification of a specific
host or release. Consult the product-owned evidence before relying on a capability.

## Projects

### codeArbiter

[![Claude Code plugin](https://img.shields.io/badge/Claude_Code-plugin-d97757)](https://github.com/arbiterForge/codeArbiter)
[![Codex plugin](https://img.shields.io/badge/OpenAI_Codex-plugin-10a37f)](https://github.com/arbiterForge/codeArbiter)
[![Pi preview](https://img.shields.io/badge/Pi-preview-d97757)](https://codearbiter.dev/getting-started/compatibility/)

A repository-owned governance layer for Claude Code, Codex CLI and Pi. Shared
procedures route implementation, reviews, decisions and delivery through explicit
lanes. Configured hooks block mediated operations; model-guided procedures and
cooperative evidence have different guarantees. Unrestricted same-user filesystem
access is outside the evidence model's protection.

The three adapters are independently packaged. Use the
[installation instructions](https://codearbiter.dev/getting-started/install/)
and [host/workflow compatibility matrix](https://codearbiter.dev/getting-started/compatibility/)
for the qualified channel, prerequisites and supported behavior. Pi remains a preview.
A source checkout, complete archive and live installed-host verification are distinct.

Repository context lives in `.codearbiter/`; integration and accounting state also
exist in Git and user-global locations. Startup can contact the configured Git
remote and GitHub. Optional tribunal feedback requires explicit per-run consent.
The [privacy policy](https://github.com/arbiterForge/codeArbiter/blob/main/PRIVACY.md)
and [security policy](https://github.com/arbiterForge/codeArbiter/blob/main/SECURITY.md)
own the full data-flow and enforcement descriptions.

See [the source](https://github.com/arbiterForge/codeArbiter) and
[published adapter releases](https://github.com/arbiterForge/codeArbiter/releases).

### arbiterIDE

arbiterIDE explores editor-owned governance as a separate product. Its development
state, platform, availability and enforcement design are maintained in the
[product repository](https://github.com/arbiterForge/arbiterIDE) and
[product site](https://arbiteride.com/). Design goals are not release evidence,
and this profile does not certify editor-level enforcement guarantees.

## License

Check each product's own terms before building on it:
[codeArbiter LICENSE](https://github.com/arbiterForge/codeArbiter/blob/main/LICENSE)
and [arbiterIDE LICENSE](https://github.com/arbiterForge/arbiterIDE/blob/main/LICENSE).
The [codeArbiter licensing and contribution policy](https://github.com/arbiterForge/codeArbiter#license-and-contributions)
owns current commercial availability and contributor-agreement status. This
profile does not grant additional rights or interpret license scope.

## Contact

Open an issue on [codeArbiter](https://github.com/arbiterForge/codeArbiter/issues) or
[arbiterIDE](https://github.com/arbiterForge/arbiterIDE/issues), or start a conversation in
[Discussions](https://github.com/orgs/arbiterForge/discussions).
