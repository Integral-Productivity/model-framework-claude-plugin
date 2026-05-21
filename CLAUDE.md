# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repo Is

A Claude Code plugin that provides skills for integrating across major models and frameworks — Integral Theory (Wilber's AQAL), developmental stage theory (Cook-Greuter EDT / LMF), Lean thinking, and similar.

## Plugin Structure

```
.claude-plugin/plugin.json   — Plugin manifest (name, version, author)
skills/<skill-name>/SKILL.md — One directory per skill; SKILL.md is the skill body
```

Skills are discovered by the Claude Code plugin loader via the `.claude-plugin/plugin.json` manifest. Each skill lives in its own subdirectory under `skills/` and is defined entirely by its `SKILL.md` file.

## SKILL.md Frontmatter

Every `SKILL.md` begins with YAML frontmatter. Recognized fields:

| Field | Purpose |
|-------|---------|
| `name` | Skill identifier (kebab-case) |
| `description` | One-line summary shown in skill listings |
| `disable-model-invocation` | If `true`, the skill content is injected as instructions without triggering a model call |

## Editorial Principle

Bridging skills are vulnerable to overreach — claiming more synthesis than the underlying scholarship supports. Every skill in this repo should:

- Distinguish *original synthesis* from established findings, and flag the synthesis explicitly.
- Cite sources with confidence; avoid making claims that hand-wave at "the literature says."
- Frame the bridge as a useful lens, not a definitive model.

## Adding a New Skill

1. Create `skills/<skill-name>/SKILL.md`.
2. Write YAML frontmatter with at least `name` and `description`.
3. Write the skill body — instructions the model follows when the skill is invoked.
