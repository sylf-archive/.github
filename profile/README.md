# Archive Repository Metadata Policy

This organization contains repositories that are no longer active and are preserved for historical, technical, or reference purposes.

To keep migrated repositories consistent, each repository should use the following minimal GitHub topics.

## Required topics

### `origin-<organization>`

Identifies the GitHub organization from which the repository was migrated.

Examples:

```text
origin-ticketmanagement
origin-cdg-tributi
origin-personal
```

Use the former organization name in lowercase and normalize spaces or separators where necessary.

### `last-used-<yyyy>`

Identifies the last year in which the repository, application, script, or project was actually used or actively maintained.

Examples:

```text
last-used-2025
last-used-2022
last-used-2019
```

This should represent the last meaningful year of use, not the year in which the repository was moved to the archive organization.

## Optional topics

### `status-<reason>`

Use only when the reason for archival adds useful information.

Recommended values:

```text
status-superseded
status-retired
status-abandoned
```

Definitions:

- `status-superseded` — replaced by another repository, application, or system.
- `status-retired` — deliberately taken out of use without necessarily having a direct replacement.
- `status-abandoned` — work stopped before the intended result was completed or adopted.

If none of these adds useful information, omit the status topic.

### `type-<kind>`

Optional classification of the repository.

Examples:

```text
type-webapp
type-api
type-library
type-script
type-tool
type-migration
type-prototype
type-documentation
```

Use this only when it helps classify the archive.

## Minimal expected metadata

The preferred minimum is therefore:

```text
origin-<organization>
last-used-<yyyy>
```

Example:

```text
origin-ticketmanagement
last-used-2024
```

When useful, add:

```text
status-superseded
type-webapp
```

Result:

```text
origin-ticketmanagement
last-used-2024
status-superseded
type-webapp
```

The goal is to keep archive metadata objective, minimal, and consistent rather than adding redundant lifecycle labels.