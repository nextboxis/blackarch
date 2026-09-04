# Copilot default prompt template (BlackArch)

Use this template when asking Copilot to make repository changes.

## Goal

- [What outcome you want]

## Context

- Repo: `nextboxis/blackarch`
- Relevant files/areas: [absolute paths or modules]
- Constraints: [tech, style, compatibility, no new dependencies, etc.]

## Done criteria

- [ ] Code changes fully implement the goal
- [ ] Existing behavior is preserved
- [ ] Focused tests are run during edits
- [ ] One full validation run is completed at the end
- [ ] Security checks are completed (secret scan + code review + CodeQL flow)
- [ ] Brief summary of what changed and why

## Execution preferences

- Start with a short plan (3-6 bullets), then execute
- Use `rg` first to narrow scope, then `view`, then edits
- Make minimal, surgical changes only
- Batch validation intelligently (avoid rerunning the full suite after tiny edits)

## Output format

1. Plan
2. Changes made
3. Validation results
4. Risks/edge cases
5. Next steps (if any)
