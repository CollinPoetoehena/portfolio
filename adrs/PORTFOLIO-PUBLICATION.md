# ADR: Keep a Single Public Portfolio of Project Profiles

## Context

The portfolio is intended to introduce a small selection of personal projects through their purpose, main techniques, organization, and project-specific lessons. It is not a complete employment portfolio or a history of every school or personal project; other work can be presented through the CV. Project repositories own their implementation and authoritative project documentation. General technical references also have authoritative sources, while some related project context is private and is not appropriate to reproduce publicly.

The portfolio therefore needs to remain focused without becoming a code mirror, a generic IT dictionary, or another copy of private project records. A profile describes a project or related set of projects, not a repository mapping: one larger repository may contain multiple related projects that belong in one profile. Profiles distinguish evidence found in authorized project sources from statements supplied by the CV.

## Decision

Maintain one small, focused public portfolio repository containing selected project profiles. Each profile may cover one project or a related set of projects, including multiple projects in one larger repository. Introduce the main techniques used, project-specific lessons, and a sufficiently detailed sanitized high-level organization; do not duplicate implementation or generic technical references. Attribute CV-supplied claims, distinguish them from independently verifiable details, and mark illustrative organization as such.

Do not create a separate private portfolio companion or attempt to represent every project or employment experience here. The CV can present other work. Source projects remain owners of their context; copying that context into a second portfolio repository would add another place to maintain without improving the selected public profiles. Keep material that is not safe and authorized for public release in its owning protected project systems. Never link to private repositories or imply that private sources are publicly accessible.

The project profile authoring process and format are documented in the [local skill](../.github/skills/project-profile-authoring/SKILL.md) and its [profile format](../.github/skills/project-profile-authoring/references/PROJECT-PROFILE-FORMAT.md).

## Consequences

### Positive

- **Selected project focus**: Readers see why a few projects exist, the techniques they use, and how they are organized without mistaking the portfolio for a complete work history.
- **Project-specific learning**: The profile format makes decisions and lessons visible while keeping authoritative implementation and detailed documentation in their owning repositories.
- **Flexible project scope**: A profile can explain related work housed in one repository without forcing a one-profile-per-repository structure.
- **Bounded publication surface**: One public repository, no private companion, and selective profiles keep publication review focused; private repository identities and evidence are not linked or disclosed.

### Negative

- **Editorial upkeep**: Profiles can become stale as project purpose and organization evolve, so evidence links and status claims need review.
- **Limited technical depth**: Readers seeking implementation detail must follow links to the owning public project, and private implementation remains unavailable.
- **Sanitization responsibility**: Public profiles still require deliberate review; a single public repository does not make accidental disclosure safe.

## Alternatives Considered

| Technique/tool (description and reference) | Advantages | Drawbacks and risks | Reason not selected | Reconsider when |
|---|---|---|---|---|
| **Selected project-profile portfolio**: maintain concise Markdown profiles for selected projects or related project sets in one public repository; see GitHub's [Markdown guidance](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax). | Connects purpose, techniques, organization, and lessons in a compact introduction; profiles can cover several related projects in a larger repository. Project owners retain detailed implementation and documentation. | Requires editorial judgment and periodic review. CV-supplied claims need attribution, while unlinked private sources limit independent public verification. | Selected because the portfolio is meant to explain a few meaningful projects, not to enumerate every project, map repositories, or expose implementation. | Reconsider profile scope if project relationships become difficult to explain or readers need a materially different presentation. |
| **Complete employment and education archive**: profile every job, school assignment, and personal project in one catalog; see GitHub's [Markdown guidance](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax). | Provides a broad chronology and a single place to browse a person's full project history. | Expands publication and maintenance scope, dilutes selected work, and can require publishing details that are better summarized for a specific audience. | The portfolio is intentionally small and focused; other experience can be presented through the CV. | Reconsider only if the portfolio obtains a distinct, explicit purpose and sustainable curation plan for a complete archive. |
| **Link directly to project repositories without profiles**: rely on repository landing pages and their documentation; see GitHub's [repository documentation](https://docs.github.com/en/repositories). | Avoids maintaining a second summary and keeps claims close to their source. | Readers must infer a project's significance from its repository; private sources are inaccessible and cannot be used as public evidence links. | A self-contained, public-safe profile gives the intended context without promising access to the source repository. | Reconsider if every selected project has an authorized public landing page that already explains its purpose and lessons. |
| **Generic technical dictionary**: organize entries around tools and concepts rather than projects; see GitHub's [Markdown documentation](https://docs.github.com/en/get-started/writing-on-github). | Could collect definitions and broad usage notes in one place. | Duplicates authoritative references, creates ongoing technical maintenance, and obscures the project work the portfolio is meant to show. | General technical background belongs in authoritative documentation; the portfolio adds value through project-specific application and lessons. | Reconsider only if the purpose changes into an intentionally maintained reference product with clear ownership. |
| **Public portfolio plus private companion**: maintain matching public and private portfolio repositories; use GitHub's [repository visibility settings](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/setting-repository-visibility) to separate access. | Could provide a private place for additional portfolio notes while retaining a public-facing edition. | Creates another repository, publication boundary, and synchronization obligation. The private project repositories already own their private context, so a companion would duplicate rather than clarify ownership. | No separate portfolio-private record is needed for the public portfolio's purpose; private project information stays with the project that owns it. | Reconsider if a distinct private portfolio process acquires a concrete owner and audience that cannot be served by the private project repositories. |
| **Code showcase or implementation mirror**: copy or aggregate project code into portfolio pages or folders. | Could let readers inspect selected implementation without opening multiple repositories. | Duplicates source of truth, risks stale or incomplete code, and expands the public disclosure surface; it also makes portfolio upkeep depend on implementation changes. | Implementation belongs in its project repository. The portfolio's differentiating value is lessons and organization, not another copy of code. | Reconsider only for a separately approved, deliberately maintained showcase with clear source ownership and publication review; it is not the current portfolio model. |

## Status

Accepted

## Date

2026-11-17
