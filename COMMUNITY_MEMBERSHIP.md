# Keptn Community membership

**Last updated:** 2021-06-01

**Disclaimer:** This document borrows heavily from the [Community Membership of OpenTelemetry](https://github.com/open-telemetry/community/blob/3f44aedd70334999b8a63586cf44f747776bddd3/community-membership.md).

This document outlines the various responsibilities of contributor roles in Keptn. 
The Keptn project consists of:
  * one **main project** with the [core services of Keptn](https://github.com/keptn/keptn)
  * **Keptn-contrib** that contains [integrations and contributions](https://github.com/keptn-contrib) for Keptn
  * **Keptn-sandbox** that new [contributions to Keptn by the community](https://github.com/keptn-sandbox) and not maintained by Keptn core maintainers 

Responsibilities for the roles in this document are scoped to the *main project* and *Keptn contrib*.

The Keptn maintainers own this document and process until delegated. They can be reached via e-mail at keptn@dynatrace.com.

| **Role**   | **Responsibilities**                                  | **Requirements**                                             | **Defined by**                                               |
| ---------- | ----------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Member     | Active contributor in the community and reviewer of PRs | Sponsored by 2 approvers or maintainers. Multiple (infrequent) contributions to the project. | [Members of the Keptn GitHub organization](https://github.com/orgs/keptn/teams/members)                           |
| Approver   | Approve contributions                       | Sponsored by 2 maintainers. Highly experienced and active member with frequent contributions. | - [Approvers of the Keptn GitHub organization](https://github.com/orgs/keptn/teams/approvers) <br>- [CODEOWNERS](https://help.github.com/en/articles/about-code-owners) in [Keptn](https://github.com/keptn/keptn) |
| Maintainer | Set direction and priorities for a subproject         | Sponsored by 2 maintainers. Demonstrates responsibility and excellent technical judgment for the whole project. | - [Maintainers of the Keptn GitHub organization](https://github.com/orgs/keptn/teams/maintainers) <br>- [CODEOWNERS](https://help.github.com/en/articles/about-code-owners) in [Keptn](https://github.com/keptn/keptn)<br> - Ownership of the GitHub repository |

**Note**: Links to *Members-, Approvers-, and Maintainers of the Keptn GitHub organization* are not publicly accessible.


## New contributors

New contributors are welcomed to the community by existing members, helped with PR workflow, and directed to relevant documentation and communication channels.

## Established community members

Established community members are expected to demonstrate their adherence to the principles in this document, familiarity with project organization, roles, policies, procedures, conventions, and technical and writing ability. Role-specific expectations, responsibilities, and requirements are enumerated below.

## Member

Members are continuously active contributors in the community. They can have issues and PRs assigned to them. Members are expected to participate in the main repository as well as in subprojects, and remain active contributors to the community.  

*Defined by:* [Member of the Keptn GitHub organization](https://github.com/orgs/keptn/people).

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
- [Open an issue](https://github.com/keptn/community/issues/new?template=membership.md&title=REQUEST%3A%20New%20membership%20for%20%3Cyour-GH-handle%3E)
  against the [keptn/community](https://github.com/keptn/community) repo:
  - Ensure your sponsors are `@mentioned` on the issue
  - Complete every item on the checklist ([preview the current version of the
    template](https://github.com/keptn/community/blob/master/.github/ISSUE_TEMPLATE/membership.md))
  - Make sure that the list of contributions included is representative of your
    work on the project.
- Have your sponsoring reviewers reply confirmation of sponsorship
- Once your sponsors have responded, your request will be reviewed by the project maintainers. Any maintainer can review the requirements and add members to the GitHub organization. 

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

*Defined by:*  [Approvers of the Keptn GitHub organization](https://github.com/orgs/keptn/teams/approvers), and [CODEOWNERS](https://help.github.com/en/articles/about-code-owners) in [Keptn](https://github.com/keptn/keptn)

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
- [Open an issue](https://github.com/keptn/community/issues/new?template=membership.md&title=REQUEST%3A%20Approver%20membership%20for%20%3Cyour-GH-handle%3E)
  against the [keptn/community](https://github.com/keptn/community) repo:
  - Ensure your sponsors are `@mentioned` on the issue
  - Complete every item on the checklist ([preview the current version of the
    template](https://github.com/keptn/community/blob/master/.github/ISSUE_TEMPLATE/membership.md))
  - Make sure that the list of contributions included is representative of your
    work on the project.

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

## Maintainer

Maintainers are the technical authority for the main repository and subproject in the Keptn project. They *MUST* have demonstrated both good judgment and responsibility towards the health of the Keptn project. Maintainers *MUST* set technical direction and make or approve design decisions for their subproject; either directly or through delegation of these responsibilities.

*Defined by:*
* [Maintainers of the Keptn GitHub organization](https://github.com/orgs/keptn/teams/maintainers)
* Ownership of the GitHub repository
* Permissions and entry in `CODEOWNERS` files

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
- [Open an issue](https://github.com/keptn/community/issues/new?template=membership.md&title=REQUEST%3A%20Maintainer%20membership%20for%20%3Cyour-GH-handle%3E)
  against the [keptn/community](https://github.com/keptn/community) repo:
  - Ensure your sponsors are `@mentioned` on the issue
  - Complete every item on the checklist ([preview the current version of the
    template](https://github.com/keptn/community/blob/master/.github/ISSUE_TEMPLATE/membership.md))
  - Make sure that the list of contributions included is representative of your
    work on the project.
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
- Ensures a healthy process for discussion and decision making is in place
- Works with other maintainers to maintain the overall project health and success
