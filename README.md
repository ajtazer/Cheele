# cheele

A Claude skill for **conversational mode**: a step-by-step discussion to understand or decide something, ending in a handoff prompt for another agent (e.g. Claude Code).

## What it does

| Behaviour | Rule |
|---|---|
| Start / resume | High-level structure first, then one part at a time |
| Format | Simple terms, short paragraphs, one point per turn |
| Interruptions | Answer the interruption, then finish the unfinished point |
| Closing points | Open until explicitly approved, rejected, acknowledged or actioned |
| Accuracy | No guessing; beliefs kept separate from verified facts |
| Scope | Out-of-scope topics are dropped for good |
| Final output | One complete handoff prompt in a single code block |

## Install

**Claude.ai / desktop app:** zip the `cheele/` folder and upload it in Claude's Skills settings.

**Claude Code:**

```bash
mkdir -p ~/.claude/skills
cp -r cheele ~/.claude/skills/
```

## Use

Type `/cheele` or say "conversational mode".
