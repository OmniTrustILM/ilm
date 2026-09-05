# Governance

ILM is governed by its maintainers, who are listed in
[MAINTAINERS.md](MAINTAINERS.md). This document describes how they are
selected, how decisions are made, and how the project is run.

## Values

- **Open by default.** Proposals, decisions, and the roadmap are recorded in
  public issues, pull requests, and discussions.
- **Security before speed.** ILM handles keys, certificates, and signatures.
  Careful review is worth more than a fast merge.
- **Extensible by design.** New capabilities are added through the public
  connector and provider interfaces, so anyone can extend the platform without
  changing its core.
- **Respectful collaboration.** Disagreement is expected; contempt is not.

## Maintainers

Maintainers are responsible for reviewing and merging contributions, guiding
the roadmap, releasing new versions, and upholding the
[Code of Conduct](https://github.com/OmniTrustILM/.github/blob/main/CODE_OF_CONDUCT.md).

Each maintainer covers one or more areas of the platform. Areas are recorded in
[MAINTAINERS.md](MAINTAINERS.md) and reflect where a maintainer reviews and
merges changes, not an exclusive ownership.

### Becoming a maintainer

Candidates are contributors with a sustained record of high-quality work on the
platform: code, review, documentation, testing, or release and infrastructure
work all count. A candidate is nominated by an existing maintainer and joins by
the vote described under [Voting](#voting).

If you would like to work towards becoming a maintainer, start with the
[contribution guide](CONTRIBUTING.md).

### Stepping down and inactivity

A maintainer may step down at any time by notifying the other maintainers.

A maintainer who has not participated in the project for six months may be
moved to emeritus status. Any maintainer may propose this, and it is decided by
the vote described under [Voting](#voting). Emeritus maintainers keep the
recognition of their past work, do not vote, and may rejoin by the vote used to
appoint a new maintainer.

### Removal

A maintainer may be removed for repeated failure to meet the responsibilities
above, or for a serious Code of Conduct violation. Prolonged inactivity is
handled by emeritus status rather than by removal. Removal is decided by the
vote described under [Voting](#voting).

## Decision making

Day-to-day decisions are made by lazy consensus in the issues, pull requests,
and discussions of the repositories in the
[OmniTrustILM](https://github.com/OmniTrustILM) organization. A change proceeds
once it is approved by at least one maintainer other than its author and no
maintainer has raised an unresolved objection.

Any maintainer may ask for a decision to be escalated to a vote. Discussions
held anywhere else are not binding; a decision only takes effect once it is
recorded in public.

## Voting

Votes are held in a public issue and stay open for at least seven days, so that
maintainers in different time zones can take part. The maintainer who called the
vote records the result when it closes.

Emeritus maintainers do not vote. A maintainer who is the subject of a vote, or
of a Code of Conduct report, does not take part in it and is not counted in its
totals.

A two-thirds majority of all maintainers is required to:

- appoint a maintainer,
- move a maintainer to emeritus status,
- remove a maintainer,
- change this document.

Any other decision that has been escalated to a vote requires a simple majority
of all maintainers.

## Code of Conduct

The project follows the
[Code of Conduct](https://github.com/OmniTrustILM/.github/blob/main/CODE_OF_CONDUCT.md)
of the OmniTrustILM organization. Violations are reported to
[ilm@omnitrust.com](mailto:ilm@omnitrust.com) and are handled by the
maintainers.

## Security

Vulnerability reports are handled by the maintainers according to the
[security policy](https://github.com/OmniTrustILM/.github/blob/main/SECURITY.md).
