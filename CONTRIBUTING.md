# Contributing

Organisation default. A repository with its own `.github/CONTRIBUTING.md` overrides this.

## Before you start

Open an issue, or claim an existing one, so two people do not build the same thing.
Anything larger than a day gets a short design note on the issue first.

## Branches

Branch from the default branch. Lowercase, hyphenated, prefixed:

| Prefix | Use |
| --- | --- |
| `feature/` | New behaviour |
| `fix/` | Bug fix |
| `hotfix/` | Urgent fix that ships outside the train |
| `chore/` | Dependencies, tooling, no behaviour change |
| `docs/` | Documentation only |
| `spike/` | Work done to answer a question, never merged as is |

Include the issue number when there is one: `feature/412-mentor-availability`.

## Commits

Conventional commits. Release notes are generated from them.

```
feat(api): return paged mentor results
fix(domain): reject reviews from students with no completed match
chore(deps): bump xunit to 2.9.2
```

Add a `Co-authored-by:` trailer when you pair.

## Which merge button

| Situation | Button |
| --- | --- |
| Branch history is worth keeping, each commit a separate decision | Merge commit |
| Branch is "wip", "fix typo", "try again" | Squash and merge |
| Small change on a branch that is behind the default | Rebase and merge |

Do not squash a long lived branch that other people have branched from. Their next merge
conflicts with every change you collapsed, and it conflicts again on the merge after
that.

## Pull requests

- Under roughly 400 changed lines. Split anything larger.
- Fill in the template. "Refactor" with no explanation gets sent back.
- CI green. Do not merge red and promise a follow up.
- `Closes #12` closes the issue on merge. If your pull request is a step rather than the
  answer, write `Refs #12`.
