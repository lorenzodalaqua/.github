---
name: Angular Component Issue
about: Adds or changes a component in an Angular project
title: "[< PROJECT >] < COMPONENT > component for < PAGE OR FEATURE >"
labels: UI
---

# Story

## Short Summary
< CONTEXT >
This issue adds the < COMPONENT > component, which < PURPOSE >.
<!--
CONTEXT: one sentence about why we need the component, e.g. "We are migrating the Reviews page to Manage Angular."
PROJECT: the project that contains the Angular app, e.g. www.analytecare.com for Manage Angular.
-->

## Acceptance Criteria
- [ ] The `< COMPONENT >` component exists, and < PAGE OR FEATURE > uses it.
- [ ] < BEHAVIOR >
- [ ] < DATA LOADING >
- [ ] < VALIDATION >
<!-- Write one criterion for each behavior. Remove the criteria that do not apply. -->

## Rationale: Pros vs. Cons
<!-- What is the rationale for the change? What are the pros and cons of the acceptance criteria? -->

### Pros
* < PRO >

### Cons
* < CON >

## Subject Matter Experts
< SUBJECT MATTER EXPERTS >
<!-- e.g. "lorenzodalaqua - Manage Angular". Add the investigator, if there was an investigation. -->

## Notes
Depends on: < API V2 AND GRAPHQL ISSUES >

< SCREENSHOTS >
<!--
Add screenshots or mockups, and mark the component on them.
Link the investigation or Epic, if there is one.
Redact all patient data in screenshots.
-->

## Applicable Standards, Conventions, etc
[Angular standards](https://github.com/Medology/Team-Standards-and-Procedures/tree/master/standards/languages/js/frameworks/angular)

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
The < COMPONENT > component is now available in < PAGE OR FEATURE >. It < PURPOSE >.
< LINK TO PR GOES HERE >
