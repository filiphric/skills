---
name: create-symlinks
description: Sync .claude and .agents by moving real files to .agents and creating symlinks in .claude. Use with /create-symlinks.
allowed-tools:
  - Read
  - Glob
  - Grep
  - Bash(find:*)
  - Bash(ls:*)
  - Bash(mkdir:*)
  - Bash(mv:*)
  - Bash(ln:*)
  - Bash(readlink:*)
  - Bash(test:*)
---

Symlinks live in the .claude directory. The real files live in the .agents directory.

Your task is to:
1. check .agents and .claude folders
2. locate any files in .claude folder that are not symlinks, move them to the .agents folder and create a symlink in the .claude folder
3. locate any files in .agents folder that do not have a symlink in the .claude folder and create symlinks

Rules:
- symlinks should be created in the .claude folder, pointing to the files in the .agents folder
- use only the tools listed in `allowed-tools` frontmatter
