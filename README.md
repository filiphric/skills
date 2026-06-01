# Agent Skills

This repository contains agent skills I created for my own projects. Each skill is installable directly from this public repository.

## Install

Install a skill with:

```sh
npx skills add filiphric/skills name-of-the-skill
```

For example:

```sh
npx skills add filiphric/skills create-symlinks
```

## Skills

| Skill | Description |
| --- | --- |
| `create-symlinks` | Syncs `.claude` and `.agents` by moving real files to `.agents` and creating symlinks in `.claude`. |

## Repository Structure

Skills live in the `skills/` directory. Each skill has its own folder containing a `SKILL.md` file:

```text
skills/
  create-symlinks/
    SKILL.md
```

## Notes

These skills are built around my own workflows, but they are public so they can be installed and adapted elsewhere.
