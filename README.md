# model-framework

A Claude Code plugin for integrating across major models and frameworks — Integral Theory (Wilber's AQAL), Ego Development Theory (Cook-Greuter / LMF), Lean thinking, and similar bodies of practice. The aim is to provide carefully-scoped bridging skills that connect one framework to another with epistemic humility ("a useful lens" rather than "the definitive model").

## Install

From the Claude Code marketplace:

```
/plugin install model-framework
```

Or add this repo directly to your plugin sources.

## What's included

- [`integral-lean-bridge`](skills/integral-lean-bridge/SKILL.md) — bridges lean thinking with Integral Metatheory (AQAL) and developmental stage theory; lenses for diagnosing why lean implementations succeed, stall, or partially install; coaching adaptations across developmental stages.

This plugin is intentionally small to start. More bridges will be added over time.

## Pairing with other plugins

The skills here describe their own subject matter without requiring other plugins, but each gains depth when paired with deeper domain plugins:

- `integral-lean-bridge` pairs naturally with the [`lean-management`](https://github.com/Integral-Productivity/lean-management) plugin's `lean-thinking` skill.

## Repo layout

```
.claude-plugin/plugin.json   — Plugin manifest
skills/<skill-name>/SKILL.md — One directory per skill; SKILL.md is the skill body
```

## License

[MIT](LICENSE).
