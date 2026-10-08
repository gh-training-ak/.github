# GitHub training

Teaching organisation for the GitHub workshops. Everything here exists to be read,
broken and rebuilt in front of a room.

## Start here

| Repository | What it is |
| --- | --- |
| [contoso-learning](https://github.com/gh-training-ak/contoso-learning) | The demo repository. A real .NET and Angular service with twenty one months of history, sprint boards, rulesets and a full `.github` folder. |

## What contoso-learning is for

It is a working service, not a slide. The code compiles with zero warnings and the test
suite runs in about a second with no database, no cache and no network. If you clone it
and the build fails, something is wrong and we want to know.

Things worth opening, in roughly this order:

1. [`.gitignore`](https://github.com/gh-training-ak/contoso-learning/blob/main/.gitignore),
   for the negation block that keeps the shared VS Code configuration while ignoring
   everybody's personal files.
2. The [`.github` folder](https://github.com/gh-training-ak/contoso-learning/tree/main/.github),
   which has far more in it than most people know is possible.
3. Pull requests
   [#33](https://github.com/gh-training-ak/contoso-learning/pull/33),
   [#34](https://github.com/gh-training-ak/contoso-learning/pull/34) and
   [#35](https://github.com/gh-training-ak/contoso-learning/pull/35), merged with the
   three different buttons so you can see what each one leaves behind.
4. The [decision records](https://github.com/gh-training-ak/contoso-learning/tree/main/docs/adr),
   including the ones that admit the shipped feature is wrong in a known way.
5. The [sprint boards](https://github.com/orgs/gh-training-ak/projects), including the
   one where nothing was delivered and the retrospective says why.

## Honesty about the demo data

The commit history is backdated, deliberately, so twenty one months of work fits in a
workshop. The fourteen contributors are invented and the email domain is
`contoso.example`, which is reserved and cannot be registered.

The Dependabot pull requests are real. Nobody wrote those.

## Defaults in this repository

Anything in a repository named `.github` becomes the organisation default for every
repository that does not have its own copy. This one supplies the contributing guide,
the code of conduct, the security policy, the support routing and the issue templates.

That is the trick worth taking home: set it once here rather than copying five files
into every new repository and watching them drift.
