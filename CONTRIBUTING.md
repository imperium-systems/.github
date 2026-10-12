# Contributing to Imperium

Thank you for your interest in Imperium. Please read this guide before opening an issue or a pull request.

## Before you start

- Imperium is **proprietary software**. By submitting a contribution, you agree to the contribution terms in section 4 of the [license](LICENSE).
- Follow the [Code of Conduct](CODE_OF_CONDUCT.md).
- For questions, use [GitHub Discussions](https://github.com/orgs/imperium-systems/discussions), not issues.
- For security problems, follow the [security policy](SECURITY.md).

## Where to contribute

| Change | Repository |
|---|---|
| A system's public interface, the catalogue, naming rules | [`imperium`](https://github.com/imperium-systems/imperium) |
| The Roblox implementation | [`roblox`](https://github.com/imperium-systems/roblox) |

A change to a public interface must land in `imperium` first. Implementations follow the reference, never the other way round.

## Naming rules

- Every system bears the Latin name of its role, and that name is the same in every engine.
- Only the casing follows the conventions of each language (`Hora.SetTime` in Luau and C#, `hora.set_time` in GDScript and Python).
- A new system must belong to one of the 12 families (Core, Curia, Forum, Aerarium, Ludus, Villa, Mundus, Theatrum, Odeum, Machina, Viae, Fabrica).

Propose new systems in Discussions (**Ideas**) before writing code.

## Pull requests

1. Open an issue or a discussion first for anything beyond a small fix.
2. Create a branch from `main`: `fix/<system>-<short-description>` or `feat/<system>-<short-description>`.
3. Keep each pull request focused on one system or one change.
4. Fill in the pull request template.
5. Make sure the code builds and existing tests pass.

## Commit messages

Use a short imperative summary, prefixed with the system name when relevant:

```
Hora: clamp SetTime to the 0–24 range
```

## Reporting bugs

Open an issue in the affected repository with the **Bug report** template, and include the system, the engine and version, and the steps to reproduce.
