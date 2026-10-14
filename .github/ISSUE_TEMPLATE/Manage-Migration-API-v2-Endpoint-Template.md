---
name: Manage Migration - API v2 Endpoint
about: Adds an API v2 endpoint that a Manage page needs for its migration to Manage Angular
title: "[api.analytecare.com] API v2 endpoint to < ACTION > < RESOURCE >"
labels: API v2
---

# Story
<!-- Procedure: https://github.com/Medology/Team-Standards-and-Procedures/blob/master/procedures/manage-angular/migrating-a-page.md -->

## Short Summary
We are migrating the < PAGE > page to Manage Angular ([investigation](< INVESTIGATION LINK >)).
This issue adds an API v2 endpoint to < ACTION > a < RESOURCE >.
<!--
ACTION: one or more of index | show | store | update | destroy | replace | bulkUpdate (see LAR1030).
RESOURCE: an Eloquent model, a Command (see LAR1031), a third-party service resource, or a file.
For a nested resource, also name the parent (e.g. "a TestCode of a NetworkTest").
-->

## Acceptance Criteria
- [ ] The endpoint follows [LAR1030] and [LAR1031].
- [ ] Access is restricted to the < ROLES > role(s), and a policy enforces it.
- [ ] Attribute names follow [LAR1035].
<!-- List each renamed attribute here, e.g. `approved` becomes `status`. -->
- [ ] The validation rules of `< LEGACY REQUEST CLASS >` (API v1) are kept.
- [ ] The attribute-level authorization of API v1 is kept, and follows [LAR1036].
- [ ] The Behat tests follow [TST1003].
<!-- For index: add one criterion for pagination, and one for each filter and sort field. -->

## Subject Matter Experts
Chekote, lorenzodalaqua - API v2 standards

## Notes
< NOTES >
<!--
Name the closest precedent, e.g. `api\v2\UniversityController` with its request, resource and policy classes.
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
None. The front end does not use this endpoint yet.

## Announcement Message
releasenotes: N/A

dev-updates:
An API v2 endpoint to < ACTION > a < RESOURCE > is available. We added it to migrate the < PAGE > page to Manage
Angular. You can also use it for other tasks.
< LINK TO PR GOES HERE >
