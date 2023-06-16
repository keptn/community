---
title: Keptn Community membership
linktitle: Membership
description: Roles and Responsibilities of Community Members
---

**Last updated:** 2021-08-26

**Disclaimer:** This document borrows heavily from the [Community Membership of OpenTelemetry](https://github.com/open-telemetry/community/blob/main/community-membership.md).

This document outlines the various responsibilities of contributor roles in Keptn. 
The Keptn project consists of:
  * one **main project** with the [core services of Keptn](https://github.com/keptn/keptn)
  * **Keptn-contrib** that contains [integrations and contributions](https://github.com/keptn-contrib) for Keptn
  * **Keptn-sandbox** that new [contributions to Keptn by the community](https://github.com/keptn-sandbox) and not maintained by Keptn core maintainers 

Responsibilities for the roles in this document are scoped to the *main project* and *Keptn contrib*.

The Keptn maintainers own this document and process until delegated. They can be reached via e-mail at keptn@dynatrace.com.

| **Role**              | **Responsibilities**                                    | **Requirements**                                                                                                                                  | **Defined by**                                                                                                                                                                                                                                                                                                                           |
|-----------------------|---------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Member                | Active contributor in the community and reviewer of PRs | Sponsored by 2 approvers or maintainers. Multiple (infrequent) contributions to the project.                                                      | [Members of the Keptn GitHub organization][Community Members] and [listed in the peribolos config][Peribolos Configuration]                                                                                                                                                                                                              |
| Subproject Approver   | Approve contributions for specific subproject           | Sponsored by 2 subproject maintainers, maintainers or higher. Highly experienced and active member with frequent contributions to the subproject. | - Member of the subproject approvers team (`https://github.com/orgs/keptn/teams/<subproject>-approvers`) and listed in the subprojects `teams.yaml` within [Peribolos Configuration Directory][Peribolos Configuration Directory]<br/>- [CODEOWNERS](https://help.github.com/en/articles/about-code-owners) in respective repositories     |
| Subproject Maintainer | Set direction and priorities for a subproject           | Sponsored by 2 subproject maintainers, maintainers or higher. Demonstrates responsibility and excellent technical judgment for the subproject.                                        | - [Approvers of the Keptn GitHub organization](https://github.com/orgs/keptn/teams/approvers) and listed within [Peribolos Configuration][Peribolos Configuration] approvers team <br>- [CODEOWNERS](https://help.github.com/en/articles/about-code-owners) in respective repositories where it makes sense                              |
| Maintainer            | Set direction and priorities for keptn                  | Sponsored by 2 maintainers or higher. Demonstrates responsibility and excellent technical judgment for the whole project.                         | - [Maintainers of the Keptn GitHub organization](https://github.com/orgs/keptn/teams/maintainers) and listed within [Peribolos Configuration][Peribolos Configuration] maintainer team<br>- [CODEOWNERS](https://help.github.com/en/articles/about-code-owners) in respective repositories where it makes sense <br>                     |

**Note**: Links to *Members-, Approvers-, and Maintainers of the Keptn GitHub organization* are not publicly accessible.
**Note**: `or higher` references technical-steering-committee, governance-committee and admins/owners 

## Definition of Subproject

A subproject:

- can consist of multiple repositories focused around the same topic
- can overlap with other subprojects repositories
- can have maintainers and approvers
- can have separate admins, which is rarely granted as this should only reflect access to security critical repository configuration.

## New contributors

New contributors are welcomed to the community by existing members, helped with PR workflow, and directed to relevant documentation and communication channels.

## Established community members

Established community members are expected to demonstrate their adherence to the principles in this document, familiarity with project organization, roles, policies, procedures, conventions, and technical and writing ability. Role-specific expectations, responsibilities, and requirements are enumerated below.

## Member

Members are continuously active contributors in the community. They can have issues and PRs assigned to them. Members are expected to participate in the main repository as well as in subprojects, and remain active contributors to the community.  

*Defined by:* [Member of the Keptn GitHub organization][Community Members].

### Requirements

- Enabled [two-factor authentication](https://help.github.com/articles/about-two-factor-authentication) on their GitHub account
- Have made multiple contributions to the project or community. Contributions may include, but is not limited to:
  - Authoring or reviewing PRs on GitHub
  - Filing or commenting on issues on GitHub
  - Contributing to the main project, subprojects, or community discussions (e.g., meetings, chat, email, and discussion forums)
- Joined the [Keptn Slack channel](https://slack.keptn.sh) 
- Have read the [contributors guide](https://github.com/keptn/keptn/blob/master/CONTRIBUTING.md)
- Sponsored by 2 approvers. Consider the following requirements for sponsors:
  - Sponsors must have close interactions with the prospective member, e.g.,
    code/design/proposal review, coordinating on issues, etc.
  - Sponsors must be approvers or maintainers in at least 1 CODEOWNERS file
    in any repository in the Keptn organization
- [Open an issue][Member Issue Request]
  against the [keptn/community][Community Repository]) repo:
  - Ensure your sponsors are `@mentioned` on the issue
  - Complete every item on the checklist ([preview the current version of the
    template][Membership Issue Template])
  - Make sure that the list of contributions included is representative of your
    work on the project.
- Have your sponsoring reviewers reply confirmation of sponsorship
- Once your sponsors have responded, your request will be reviewed by the project maintainers. Any maintainer can review the requirements and add members to the GitHub organization. 
- Add yourself to the list of organization members within the [Peribolos Configuration][Peribolos Configuration]

### Responsibilities and privileges

- Is responsive to assigned issues and PRs
- Is an active owner of contributed code (unless ownership is explicitly transferred)
  - Code is well tested
  - Tests consistently pass
  - Addresses bugs or issues discovered after code is accepted
- Can review and approve via the GitHub workflow. This review work is
  not sufficient to merge a PR. There will still need to be a review by an
  *approver*.
- Can be assigned to issues and PRs, and people can ask members for
  reviews with a `/cc @username`.

**Note:** Members who frequently contribute code are expected to proactively perform code reviews and work towards becoming an *approver* for the main repository or subproject that they are active in. Acceptance of code contributions requires at least one approver in addition to the reviews by *members*.

## Approver

Code approvers are able to both review and approve code contributions, as well as help maintainers triage issues and do project management. While code review is focused on code quality and correctness, approval is focused on holistic acceptance of a contribution including: backwards/forwards compatibility, adhering to API and flag conventions, subtle performance and correctness issues, interactions with other parts of the system, etc.

*Defined by:* Member of the subproject approvers team (`https://github.com/orgs/keptn/teams/<subproject>-approvers`) and listed in the subprojects `teams.yaml` within [Peribolos Configuration Directory][Peribolos Configuration Directory]

Approver status can be scoped to a part of the codebase. For example, critical core components may have higher bar of becoming an approver. Some approvers may only be doing issues triage and do not have approval rights.

### Requirements

*The following applies to the part of the codebase for which one would be an approver in the `CODEOWNERS` file:*

- Reviewer of the codebase for at least 1 month
- Reviewer for or author of at least 10 substantial PRs to the codebase,
  with the definition of substantial subject to the maintainer's discretion
  (e.g., refactors/adds new functionality rather than one-line pulls).
- Sponsored by 2 maintainers. Consider the following requirements for sponsors:
  - No objections from other maintainers
  - Done through a PR that updates the corresponding `CODEOWNERS` file
- [Open an issue][Approver Issue Request]
  against the [keptn/community][Community Repository]) repo:
  - Ensure your sponsors are `@mentioned` on the issue
  - Complete every item on the checklist ([preview the current version of the
    template][Membership Issue Template])
  - Make sure that the list of contributions included is representative of your
    work on the project.
- Add yourself to the list of approvers for the respective subproject within [Peribolos Configuration Directory][Peribolos Configuration Directory]

### Responsibilities and privileges

*The following applies to the part of the codebase for which one would be an approver in the `CODEOWNERS` file:*

- Approver status may be a precondition to accepting large code contributions
- Demonstrates sound technical judgment
- Approves code contributions for acceptance
- Is responsible for project quality control via code reviews:
  - Focus on holistic acceptance of contribution such as dependencies with other
    features, backwards / forwards compatibility, API and flag definitions, etc.
- Is expected to be responsive to review requests - inactivity for more than 1 month may result in suspension until active again
- Is mentor of new members

## Subproject Maintainer

Maintainers are the technical authority for subproject repositories and subproject in the Keptn project. They *MUST* have demonstrated both good judgment and responsibility towards the health of the Keptn project. Maintainers *MUST* set technical direction and make or approve design decisions for their subproject; either directly or through delegation of these responsibilities.

*Defined by:*
* Member of the subproject maintainer team (`https://github.com/orgs/keptn/teams/<subproject>-maintainer`) and listed in the subprojects `teams.yaml` within [Peribolos Configuration Directory][Peribolos Configuration Directory]

### Requirements

The process for becoming a maintainer should be defined in the project or subproject. Unlike the roles outlined above, the owners of a subproject are typically limited to a relatively small group of decision makers and updated as fits the needs of the subproject.

*The following applies to the subproject for which one would be an owner:*

- Deep understanding of the technical goals and direction of the subproject
- Deep understanding of the technical domain (specifically the language) of the subproject
- Sustained contributions to design and direction by doing all of:
  - Authoring and reviewing proposals
  - Initiating, contributing, and resolving discussions (e-mails, GitHub issues,
    meetings)
  - Identifying subtle or complex issues in designs and implementation PRs
- Directly contributed to the subproject through implementation and / or review
- Aligning with the overall project goals, specifications, and design principles. Bringing general questions and requests to the discussions as part of the specifications project.
- [Open an issue][Membership Issue Request]
  against the [keptn/community][Community Repository]) repo:
  - Ensure your sponsors are `@mentioned` on the issue
  - Complete every item on the checklist ([preview the current version of the
    template][Membership Issue Template])
  - Make sure that the list of contributions included is representative of your
    work on the project.
  - Add yourself to the list of approvers for the respective subproject within [Peribolos Configuration Directory][Peribolos Configuration Directory]

### Responsibilities and privileges

*The following applies to the subproject for which one would be an owner:*

- Makes and approves technical design decisions for the subproject
- Sets technical direction and priorities for the subproject
- Defines milestones and releases
- Is mentor and guides approvers, and maintainers to the subproject
- Escalates *reviewer* and *maintainer* workflow concerns (i.e., responsiveness, availability, and general contributor community health) to the TC.
- Ensures continued health of subproject:
  - Adequate test coverage to confidently release
  - Tests are passing reliably (i.e., not flaky) and are fixed when they fail
- Ensures a healthy process for discussion and decision-making is in place
- Works with other maintainers to maintain the overall project health and success

## Maintainer

Maintainers are the technical authority for all subprojects within the Keptn project. They *MUST* have demonstrated both good judgment and responsibility towards the health of the Keptn project. Maintainers *MUST* set technical direction and make or approve design decisions for the overall project; either directly or through delegation of these responsibilities.

*Defined by:*
* [Maintainers of the Keptn GitHub organization](https://github.com/orgs/keptn/teams/maintainers) and listed within [Peribolos Configuration][Peribolos Configuration] maintainer team

### Requirements

As `Maintainer` has the same requirements as a `subproject Maintainer` but those apply on a global level.

- Deep understanding of the technical goals and direction of the subprojects
- Deep understanding of the technical domain (specifically the language) of the subprojects
- Sustained contributions to design and direction by doing all of:
  - Authoring and reviewing proposals
  - Initiating, contributing, and resolving discussions (e-mails, GitHub issues,
    meetings)
  - Identifying subtle or complex issues in designs and implementation PRs
- Directly contributed to subprojects through implementation and / or review
- Aligning with the overall project goals, specifications, and design principles. Bringing general questions and requests to the discussions as part of the specifications project.
- [Open an issue][Membership Issue Request]
  against the [keptn/community][Community Repository]) repo:
  - Ensure your sponsors are `@mentioned` on the issue
  - Complete every item on the checklist ([preview the current version of the
    template][Membership Issue Template])
  - Make sure that the list of contributions included is representative of your
    work on the project.
  - Add yourself to the list of approvers for the respective subproject within [Peribolos Configuration Directory][Peribolos Configuration Directory]

### Responsibilities and privileges

- Makes and approves technical design decisions for subprojects
- Sets technical direction and priorities for subprojects
- Defines milestones and releases
- Is mentor and guides approvers, and maintainers to subprojects
- Escalates *reviewer* and *maintainer* workflow concerns (i.e., responsiveness, availability, and general contributor community health) to the TC.
- Ensures continued health of subprojects:
  - Adequate test coverage to confidently release
  - Tests are passing reliably (i.e., not flaky) and are fixed when they fail
- Ensures a healthy process for discussion and decision-making is in place
- Works with other maintainers to maintain the overall project health and success

[Community Members]: https://github.com/orgs/keptn/people
[Community Repository]: https://github.com/keptn/community
[Peribolos Configuration]: ./config/keptn/org.yaml
[Peribolos Configuration Directory]: ./config/keptn/
[Membership Issue Template]: https://github.com/keptn/community/blob/master/.github/ISSUE_TEMPLATE/membership.md
[Maintainer Issue Request]: https://github.com/keptn/community/issues/new?template=membership.md&title=REQUEST%3A%20Maintainer%20membership%20for%20%3Cyour-GH-handle%3E
[Approver Issue Request]: https://github.com/keptn/community/issues/new?template=membership.md&title=REQUEST%3A%20Approver%20membership%20for%20%3Cyour-GH-handle%3E
[Member Issue Request]: https://github.com/keptn/community/issues/new?template=membership.md&title=REQUEST%3A%New%20=membership%20for%20%3Cyour-GH-handle%3E


## Inactivity

It is important for contributors to be and stay active to set an example and show commitment to the project. Inactivity is harmful to the project as it may lead to unexpected delays, contributor attrition, and a loss of trust in the project.

- Inactivity is measured by:
  - Periods of no contributions for longer than 3 months
  - Periods of no communication for longer than 3 months
- Consequences of being inactive include:
  - Involuntary removal or demotion
  - Being asked to move to Emeritus status

## Involuntary Removal or Demotion

Involuntary removal/demotion of a contributor happens when responsibilities and requirements aren't being met. This may include repeated patterns of inactivity, extended periods of inactivity, a period of failing to meet the requirements of your role, and/or a violation of the Code of Conduct. This process is important because it protects the community and its deliverables while also opening up opportunities for new contributors to step in.

Involuntary removal or demotion is handled through a vote by a majority of the current Maintainers.

## Stepping Down/Emeritus Process

If and when contributors' commitment levels change, contributors can consider stepping down (moving down the contributor ladder) vs moving to emeritus status (completely stepping away from the project).

Contact the Maintainers about changing to Emeritus status, or reducing your contributor level.

When a contributor returns to being more active, they may be promoted back to their previous position at the discretion of the current maintainers by opening a PR. If the current maintainers do not agree to restoring the previous responsibilities, they should follow the contributor ladder steps.
