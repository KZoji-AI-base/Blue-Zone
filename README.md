# Blue-Zone (personal workspace)

Personal working repository for Blue Zone–related tasks that are kept separate from the
organization repositories. Drafts, experiments, scripts, research notes and handoffs live here
until they are ready to move to a shared location.

> **Visibility:** this repository is intended to be **private**. Do not commit credentials,
> guest/tenant/resident personal data, contracts, financials or HR material. See
> [Privacy rules](#privacy-rules).

## Layout

| Folder | What goes here |
| --- | --- |
| `projects/` | One subfolder per piece of work (`projects/YYYY-MM-short-name/`), each with its own `README.md` from the template |
| `notes/` | Loose notes, research, meeting takeaways, ideas not yet a project |
| `scripts/` | Reusable scripts and small tools (automation, data cleanup, exports) |
| `handoffs/` | Handoff files for continuing work in a new Claude session (`YYYY-MM-DD-topic.md`) |
| `templates/` | Starting points for project READMEs and handoffs |
| `archive/` | Finished or abandoned work, kept for reference |

## Conventions

- **Naming:** lowercase, hyphenated, date-prefixed where order matters
  (`2026-11-wifi-survey/`, `2026-11-10-handoff-site-copy.md`).
- **Language:** Japanese deliverables are written in Japanese (not translated); English uses
  American spelling. Bilingual material keeps both versions side by side (`*.ja.md`, `*.en.md`).
- **Status:** every project README starts with a status line: `draft`, `active`, `paused`,
  `done` or `moved` (with a link to where it moved).
- **Sources:** record whether a claim is measured, recorded or inferred, and link the source.
- **Branches:** `main` holds the current state. Claude sessions work on `claude/*` branches and
  open draft pull requests for review.

## Starting something new

```bash
cp -r templates/project projects/2026-11-short-name
```

Then fill in the project's `README.md` (goal, status, sources, next steps).

## Privacy rules

1. No secrets: API keys, passwords, tokens and `.env` files stay out of git (`.gitignore`
   covers the common ones). Use the environment's secret store or a password manager.
2. No personal data about guests, tenants, students, staff or applicants. Use anonymized or
   synthetic samples.
3. No confidential business documents (contracts, financials, HR files). Reference them by
   location instead of copying them in.
4. Personal and health material stays out of this repository entirely.
5. Before sharing anything from here, move it to the appropriate organization repository or
   document store.
