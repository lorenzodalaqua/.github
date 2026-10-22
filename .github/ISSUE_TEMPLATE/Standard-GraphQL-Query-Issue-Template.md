---
name: GraphQL Query Issue
about: Adds or changes a GraphQL query in api.analytecare.com
title: "[api.analytecare.com] GraphQL query for < MODEL > and its relationships"
labels: GraphQL
---

# Story

## Short Summary
< CONTEXT >
This issue makes sure that a GraphQL query for < MODEL > exists, with the relationships that < CLIENT > needs.
<!--
CONTEXT: one sentence about why we need the query, e.g. "We are migrating the Reviews page to Manage Angular."
CLIENT: the page or feature that uses the query.
-->

## Acceptance Criteria
- [ ] The < MODEL > query follows [LAR1032], [LAR1033] and [LAR1034].
<!-- State the query kind: singular, list, or both. -->
- [ ] These relationships are exposed: < RELATIONSHIP PATHS >
<!-- Use dotted paths with the GraphQL field names, e.g. `network.network_accounts`. -->
- [ ] The field names follow [LAR1035].
- [ ] The restricted fields (< RESTRICTED FIELDS >) follow [LAR1036].
<!-- Write "None" if no field is restricted. -->
- [ ] The Behat tests follow [TST1002].

## Subject Matter Experts
Chekote, lorenzodalaqua - GraphQL standards

## Notes
If a legacy query conflicts with a standard, coordinate with the leads.
<!--
Link the investigation or Epic, if there is one.
Add other information that is specific to this query.
-->

## Applicable Standards, Conventions, etc
[LAR1032], [LAR1033], [LAR1034], [LAR1035], [LAR1036], [TST1002]

[LAR1032]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/graphql/LAR1032-graphql-query-naming.md
[LAR1033]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/graphql/LAR1033-graphql-list-queries-paginated.md
[LAR1034]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/graphql/LAR1034-graphql-query-authorization.md
[LAR1035]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/LAR1035-api-attribute-naming.md
[LAR1036]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/LAR1036-attribute-level-authorization.md
[TST1002]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/testing/TST1002-behat-graphql-feature-files.md

## Exploratory Testing
< EXPLORATORY TESTING >
<!--
If no client uses the query yet, write "None. No client uses this query yet."
Otherwise, list the projects and features that use it, e.g. "www.analytecare.com - Manage Angular - Reviews".
-->

## Announcement Message
releasenotes: N/A

dev-updates:
A GraphQL query for < MODEL > and its relationships is available. We added it to < REASON >.
You can also use it for other tasks.
< LINK TO PR GOES HERE >
