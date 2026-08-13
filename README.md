# upstream-defect-report-rulebook

Rulebook for the `upstream-defect-report` role (contract v3 role-handoff
protocol). Seeded directly with its operational playbook per
`docs/issue-1174/proposals/operational-playbook-program.md` (parent repo
`tokenmaxxxer/on-the-record`) — this role had no prior rulebook repo, so
it lands under proposal section (d)'s no-existing-repo path: create the
repo now rather than defer, so the playbook has a landing home matching
the other 43 role rulebooks.

## Layout

- `playbook/subtraction.md` — what to cut from a defect report before
  filing (condition → choice → source rules)
- `playbook/comprehensibility.md` — structuring a report a stranger
  maintainer can parse on first read
- `playbook/convention.md` — matching the specific upstream project's
  own stated and de facto process

Each file carries `axis:`/`rule_count_floor:` front matter for
`gates/playbook_depth_gate.py` (parent repo) to read, per the operational
program's spec (c). Role floor = 3 axes × sparse-tier multiplier(1),
`max(5, 3×1) = 5` per axis (this role's own scout pass found a *bounded*
public literature — Nature/PLOS/Sweller-level, not a large citable
canon — closer to "sparse" than "moderate"); each axis file exceeds its
per-axis floor of 5 to leave margin for the human depth spot-check.
Each axis includes at least one `removal`-classified rule block (choice
verb: cut/drop/delete/omit, or 삭제/생략/줄이다), per amendment 4.

This is a playbook-only seed, not a finished rulebook: no plugin/gate
scaffolding (`.claude-plugin/`, `hooks/`) has been added yet, since this
issue's own program scope was "write the playbook," not "stand up the
full role-taxonomy plugin skeleton" (a separate, unrelated issue chain
per the sibling rulebooks' own history — see e.g.
`finance-unit-economics-rulebook`'s issue-170 seed commit).
