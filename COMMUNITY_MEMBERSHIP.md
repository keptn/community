# Contributor Ladder

**Disclaimer:** This document borrows heavily from the [Community Membership of OpenTelemetry](https://github.com/open-telemetry/community/blob/3f44aedd70334999b8a63586cf44f747776bddd3/community-membership.md).

**Ownership:** This document is owned by the Governance committee, Technichal committee and community manager [ADD LINK TO GOVERNACE AND TC]().

Hello! We are excited that you want to learn more about our project contributor ladder! This contributor ladder outlines the different contributor roles within the project, along with the responsibilities and privileges that come with them. Community members generally start at the first levels of the "ladder" and advance up it as their involvement in the project grows. Our project members are happy to help you advance along the contributor ladder.

Each of the roles is organized into lists of three types of things. "Responsibilities" are things that a contributor is expected to do. "Requirements" are qualifications a person needs to meet to be in that role, and "Privileges" are things contributors on that level are entitled to.

## Community Participant

A Community Participant engages with the project and its community, contributing their time, thoughts, etc. Community participants are usually users who have stopped being anonymous and started being active in project discussions.

- Responsibilities:
  - Must follow the [CNCF CoC](https://github.com/cncf/foundation/blob/main/code-of-conduct.md)
- How users can get involved with the community:
  - Participating in community discussions
  - Submitting bug reports
  - Commenting on issues
  - Trying out new releases
  - Attending community events
  - Reviewing pull requests

## Contributor

A Contributor contributes directly to the project and adds value to it. Contributions need not be code. People at the Contributor level may be new contributors, or they may only contribute occasionally.

- Responsibilities include:
  - Follow the [CNCF CoC](https://github.com/cncf/foundation/blob/main/code-of-conduct.md)
  - Follow the project contributing guide
- Requirements (one or several of the below):
  - Report and sometimes resolve issues
  - Occasionally submit PRs
  - Contribute to the documentation
  - Show up at meetings, takes notes
  - Answer questions from other community members
  - Submit feedback on issues and PRs
  - Test releases and patches and submit reviews
  - Run or helps run events
  - Promote the project in public
  - Help run the project infrastructure
- Privileges:
  - Invitations to contributor events
  - Eligible to become an Organization Member


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
- Add yourself to the list of [project members](https://github.com/keptn/keptn/blob/master/MAINTAINERS)

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
- Add yourself to the list of [project approvers](https://github.com/keptn/keptn/blob/master/MAINTAINERS)

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
- Add yourself to the list of [project members](https://github.com/keptn/keptn/blob/master/MAINTAINERS)
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
