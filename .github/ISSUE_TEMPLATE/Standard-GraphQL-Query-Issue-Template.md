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
- [ ] The < MODEL > query follows [LAR1032] and [LAR1033].
<!-- State the query kind: singular, list, or both. -->
- [ ] A policy authorizes the query.
- [ ] These relationships are exposed: < RELATIONSHIP PATHS >
<!-- Use dotted paths with the GraphQL field names, e.g. `network.network_accounts`. -->
- [ ] The field names follow [LAR1034].
- [ ] The policy authorizes the restricted fields (< RESTRICTED FIELDS >).
<!-- Write "None" if no field is restricted. -->
- [ ] The Behat tests follow [TST1002].

## Rationale: Pros vs. Cons
<!-- What is the rationale for the change? What are the pros and cons of the acceptance criteria? -->

### Pros
* < PRO >

### Cons
* < CON >

## Subject Matter Experts
Chekote, lorenzodalaqua - GraphQL standards

## Notes
If a legacy query conflicts with a standard, coordinate with the leads.
<!--
Link the investigation or Epic, if there is one.
Add other information that is specific to this query.
-->

## Applicable Standards, Conventions, etc
* [GraphQL standards](https://github.com/Medology/Team-Standards-and-Procedures/tree/master/standards/languages/php/frameworks/laravel/api/graphql)
* [Standards for API v2 and GraphQL](https://github.com/Medology/Team-Standards-and-Procedures/tree/master/standards/languages/php/frameworks/laravel/api)
* [Testing standards](https://github.com/Medology/Team-Standards-and-Procedures/tree/master/standards/testing)

[LAR1032]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/graphql/LAR1032-graphql-query-naming.md
[LAR1033]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/graphql/LAR1033-graphql-list-queries-paginated.md
[LAR1034]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/LAR1034-api-attribute-naming.md
[TST1002]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/testing/TST1002-behat-graphql-feature-files.md

## Exploratory Testing
`A comprehensive list of the areas of this project that are affected by this PR`

The following API endpoints are affected by this change: (if this issue is for an API project)

* `API ROUTE`
* `API ROUTE`
* `etc`

The following features/pages are affected by this change: (If applicable)

* `PROJECT NAME - FEATURE NAME`
* `PROJECT NAME - FEATURE NAME`
* `etc`

Note: You should include all projects that are affected by this, not just the project that the PR was submitted to. For example, if you make a change that affects an AnalyteCare API endpoint, then you'll want to use our observability tools such as Google Cloud Logging to determine which clients are using that endpoint, and then coordinate with the SMEs (if necessary) to determine which features that project is using the API endpoint to facilitate, and list those here for QA to test.

## Announcement Message
releasenotes: N/A

dev-updates:
A GraphQL query for < MODEL > and its relationships is available. We added it to < REASON >.
You can also use it for other tasks.
< LINK TO PR GOES HERE >
