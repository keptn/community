GSoC 2022 - Entity Custom Resource Definitions for Keptn GitOps
==========

This project implements the remaining Keptn entities as Kubernetes Custom Resource Definitions
to shift more of Keptn's components towards a GitOps workflow.
As a result, users will be able to configure these entities 
via PRs to a configuration repository or manage them directly using the Kubernetes APIs.

## Project team

- Contributor: Eric Y. Kim - [GitHub](https://github.com/eyskim) | [LinkedIn](https://www.linkedin.com/in/eykim195/)

- Mentors:
Thomas Schuetz,
Suraj Banakar,
Afzal Ansari

## Contacts

- Slack: `#wg-keptn-gitops-operator` on [Keptn Slack](https://keptn.sh/community/#slack)

## Details

There has been significant progress towards a fully GitOps approach for Keptn through the implementation of the [Keptn Gitops Operator Prototype](https://github.com/keptn-sandbox/keptn-gitops-operator). In fact, it is already possible to configure Keptn by merging pull requests to a configuration repository and by application of the following [Kubernetes Custom Resources (CRs)](https://github.com/keptn-sandbox/keptn-gitops-operator#custom-resources):
- KeptnInstance
- KeptnProject
- KeptnService
- KeptnSequence
- KeptnStage
- KeptnServiceDeployment

Along with this progress, there are additional possible enhancements discussed in [discussions/5296](https://github.com/keptn/keptn/discussions/5296) to achieve a Keptn workflow that includes configuration via the Kubernetes API and less frequent communication with the Keptn upstream repository. Specifically, this project will implement the outstanding Keptn entity CRs not currently included in the prototype:
- SLI configs
- SLO configs
- Remediation configs
- Webhook configs

As a result, in addition to bringing Keptn closer to achieving a GitOps workflow, users will benefit as a result of:
- Improved performance due to less frequent communication with the Keptn Git repository (as already mentioned)
- Added ability to manage Keptn entities directly using kubectl

## References

* [Project page on the GSoC website](https://summerofcode.withgoogle.com/programs/2022/projects/yd9z3DBo)
