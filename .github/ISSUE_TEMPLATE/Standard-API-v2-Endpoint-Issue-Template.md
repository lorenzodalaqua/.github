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
- [ ] Attribute names follow [LAR1035].
<!-- List each renamed attribute here, e.g. `approved` becomes `status`. -->
- [ ] The Behat tests follow [TST1003].
<!--
For index: add one criterion for pagination, and one for each filter and sort field.
If this endpoint replaces an API v1 endpoint, add:
- [ ] The validation rules of `< LEGACY REQUEST CLASS >` (API v1) are kept.
- [ ] The attribute-level authorization of API v1 is kept, and follows [LAR1036].
-->

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
[LAR1030], [LAR1031], [LAR1035], [LAR1036], [TST1003]

[LAR1030]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/v2/LAR1030-api-v2-rest.md
[LAR1031]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/v2/LAR1031-api-v2-command-resources.md
[LAR1035]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/LAR1035-api-attribute-naming.md
[LAR1036]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/languages/php/frameworks/laravel/api/LAR1036-attribute-level-authorization.md
[TST1003]: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/standards/testing/TST1003-behat-api-v2-feature-files.md

## Exploratory Testing
< EXPLORATORY TESTING >
<!--
If no client uses the endpoint yet, write "None. No client uses this endpoint yet."
Otherwise, list the projects and features that use it, e.g. "www.analytecare.com - Manage Angular - Reviews".
-->

## Announcement Message
releasenotes: N/A

dev-updates:
An API v2 endpoint to < ACTION > a < RESOURCE > is available. We added it to < REASON >.
You can also use it for other tasks.
< LINK TO PR GOES HERE >
