---
name: API v2 Endpoint Issue
about: Adds or changes an API v2 endpoint in api.analytecare.com
title: "[api.analytecare.com] API v2 endpoint to < ACTION > < RESOURCE >"
labels: API v2
---

# Story

## Short Summary
< CONTEXT >
This issue adds an API v2 endpoint to < ACTION > a < RESOURCE >.
<!--
CONTEXT: one sentence about why we need the endpoint, e.g. "We are migrating the Reviews page to Manage Angular."
or "My Account must show the subscriptions of an account."
ACTION: one or more of index | show | store | update | destroy | replace | bulkUpdate (see LAR1030).
RESOURCE: an Eloquent model, a Command (see LAR1031), a third-party service resource, or a file.
For a nested resource, also name the parent (e.g. "a TestCode of a NetworkTest").
-->

## Acceptance Criteria
- [ ] The endpoint follows [LAR1030] and [LAR1031].
- [ ] Access is restricted to the < ROLES > role(s), and a policy enforces it.
- [ ] Attribute names follow [LAR1034].
<!-- List each renamed attribute here, e.g. `approved` becomes `status`. -->
- [ ] The Behat tests follow [TST1003].
<!--
For index: add one criterion for pagination, and one for each filter and sort field.
If this endpoint replaces an API v1 endpoint, add:
- [ ] The validation rules of `< LEGACY REQUEST CLASS >` (API v1) are kept.
- [ ] The attribute-level authorization of API v1 is kept.
-->

## Rationale: Pros vs. Cons
<!-- What is the rationale for the change? What are the pros and cons of the acceptance criteria? -->

### Pros
* < PRO >

### Cons
* < CON >

## Subject Matter Experts
Chekote, lorenzodalaqua - API v2 standards

## Notes
< NOTES >
<!--
Name the closest precedent, e.g. `api\v2\UniversityController` with its request, resource and policy classes.
Link the investigation or Epic, if there is one.
Add other information that is specific to this endpoint. Write "None" if there is none.
-->

## Applicable Standards, Conventions, etc
* [API v2 standards](https://github.com/Medology/Team-Standards-and-Procedures/tree/master/standards/languages/php/frameworks/laravel/api/v2)
* [Standards for API v2 and GraphQL](https://github.com/Medology/Team-Standards-and-Procedures/tree/master/standards/languages/php/frameworks/laravel/api)
* [Testing standards](https://github.com/Medology/Team-Standards-and-Procedures/tree/master/standards/testing)

[LAR1030]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/v2/LAR1030-api-v2-rest.md
[LAR1031]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/v2/LAR1031-api-v2-command-resources.md
[LAR1034]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/LAR1034-api-attribute-naming.md
[TST1003]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/testing/TST1003-behat-api-v2-feature-files.md

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
An API v2 endpoint to < ACTION > a < RESOURCE > is available. We added it to < REASON >.
You can also use it for other tasks.
< LINK TO PR GOES HERE >
