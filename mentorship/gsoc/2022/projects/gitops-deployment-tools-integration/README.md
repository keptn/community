<div align="center">
<img src="https://raw.githubusercontent.com/iamrajiv/GSoC-2022/main/assets/gsoc-2022-1.svg" height="auto" width="600" />
<br />
<img src="https://raw.githubusercontent.com/iamrajiv/GSoC-2022/main/assets/gsoc-2022-2.svg" height= "auto" width="400" />
<br />
<h1>Keptn</h1>
<h3>
Integration for GitOps-based Deployment Tools (ArgoCD/Flux)
</h3>
</div>

## Table of Contents

- [Introduction](#introduction)
- [Project team](#project-team)
- [Contacts](#contacts)
- [Work Summary](#work-summary)
- [Challenges](#challenges)
- [Acknowledgments](#acknowledgments)
- [References](#references)

## Introduction

To be able to use GitOps tools in combination with Keptn.
The main goal of this project is to find a proper way how the tools could interact with Keptn and to build an integration for such tools.

Deployment tools can be integrated via the helm-service or via the job-executor service.

Currently, there’s no way to integrate GitOps Tools in Keptn. Provide a way such that such tools can be integrated into Keptn return deployment states after the state has been synced.

This project would be done in collaboration with Flux and Keptn maintainers.

## Project team

- Contributor: Meha Bhalodiya - [GitHub](https://github.com/mehabhalodiya) | [LinkedIn](https://www.linkedin.com/in/meha-bhalodiya) | [Twitter](https://twitter.com/mehabhalodiya)
- Mentors:
    - Brad McCoy - [GitHub](https://github.com/bradmccoydev) | [LinkedIn](https://www.linkedin.com/in/bradmccoy3/) | [Twitter](https://twitter.com/bradmccoydev)
    - Thomas Schuetz - [GitHub](https://github.com/thschue) | [LinkedIn](https://www.linkedin.com/in/thschue/) | [Twitter](https://twitter.com/ThSchue)

## Contacts

- Slack: `#wg-keptn-gitops-operator` on [Keptn Slack](https://keptn.sh/community/#slack)

## Project Details

As adopters of Keptn move to a GitOps paradigm in their organization it is essential that for the deployment purpose they use Argo/Flux by integrating it in the [keptn/keptn](https://github.com/keptn/keptn) workflow.

As a project that is about to be incubated into the CNCF, it is even more important now to make adoption as seamless as possible. One thing which also might be stated is that many people like to use Argo/Flux and it would bring a huge benefit to the ecosystem when keptn as an orchestrator could deal with this.

The main benefits of integrating this would be that tooling would get changeable. For instance, you can change from Argo to Flux without changing your
testing strategy. Furthermore, it would allow users to use keptn without touching their current deployment tooling.

## Work Summary

A few major milestones of this project were as follows:
- Finding a way to integrate GitOps Tools in keptn
- Provide an integration service for such tools
- Provide documentation on how to use this integration
- Creating a testing pipeline for new versions and compatibility

## Challenges
Various challenges were faced during the project. Some are

- Make the alert and provider in the working state
- Matching the provider labels as in the project
- Getting `Release reconciliation succeeded` status of the demo 

Scheduling meetings like mentors and mentees were at different time zones so it was a little bit hard to sync up but we did it and we had a great meeting.

## Learnings
I am very glad that I had the opportunity to take part in the Google Summer of Code program. Participating in this program has helped me to:

- Proper PoC and understanding are very important before starting the project or any feature and also we should have other alternatives before choosing the best one. This thing I got to learn when the `Upgrading version of the demo and triggering the event` feature was not implemented fully because I did not understand the feature properly.
- Learned about Keptn and it's CLI functionality, Helm, Flux, etc.
- Planning and structuring the requirements for the project and managing high-priority tasks and low-priority tasks.
- How to work in a team and how to communicate with the team.

Apart from the above, I have learned a lot of things from my mentors and other community members. I am very thankful to my mentors and other community members for helping me throughout the program.

## Acknowledgments
I am deeply grateful to my mentors [Brad McCoy](https://github.com/bradmccoydev) and [Thomas ](https://github.com/thschue) for guiding me through the project and were always ready to help, review work in progress, gave feedback regarding the overall shape of the project and the feasibility of certain solutions and maintained a very friendly, supportive, and stimulating atmosphere on the team. They devoted a lot of time to this project. 

I'd also like to thank [Oleg Nenashev](https://github.com/oleg-nenashev) and [Keptn](https://github.com/keptn/keptn) community members for their support and feedback.

Last but not least, I would like to thank Google and Google Summer of Code organizers for this initiative.

## References
* [Enhancement Proposal](https://github.com/keptn/enhancement-proposals/pull/67)
* [Contributor Proposal link](https://docs.google.com/document/d/194yMNDTolmMSxBkXD_1HcfmtOaB0N7AlMfVPSI0yc60/edit?usp=sharing)
* [Project page at GSoC 2022 website](https://summerofcode.withgoogle.com/programs/2022/projects/yHHRfVz2)
* [GitHub Project Board (timeline & issues)](https://github.com/keptn-sandbox/keptn-flux-integration/projects/1)
* [Meeting Notes & Updates](https://docs.google.com/document/d/1AWTQdsJPJpZUgmY3qJ-QHewHvEukt7aHQTOJtnYsxVQ/edit?usp=sharing)
* [Keptn GitOps support for Flux: issue link](https://github.com/keptn/integrations/issues/28)
* [Project repository](https://github.com/keptn-sandbox/keptn-flux-integration)
* [Contributor repository](https://github.com/mehabhalodiya/GSoC-22) 

<div align="right">
<img src="https://raw.githubusercontent.com/iamrajiv/GSoC-2022/main/assets/gsoc-2022-3.svg" height="auto" width="100" />
</div>
