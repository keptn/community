# GSoC Project Ideas - Keptn

This document presents Google Summer of Code project ideas
which Keptn contributors have proposed for this year.
Application guidelines and more information about Keptn
in GSoC are available on [this page](../README.md)

## 2024 Project Ideas

- [GitHub issue self-assignment bot](#github-issue-self-assignment-bot)

### GitHub issue self-assignment bot

- Description: The goal is to create a self-service issue assignment bot for GitHub contributors who are not yet part of the organization but would like to work on issues marked for external handling. The bot should be able to check if the user is part of the organization, examine if the pre-conditions for self-assignment are met (configurable labels or rules about number of issues already assigned/PRs opened), and assign the issue. Additionally, the bot should be able to track the state of the issue by adding/removing specific labels. The bot should be part of the CI and executed as an action on an issue change.
- Expected Outcome:
  - Implement GitHub bot in TypeScript/Golang
  - Bot does not require an external hosting
  - Bot is able to assign GitHub issues to contributors following the pre-defined set of rules
  - Bot is able to track the status of GitHub issues with labels
  - Introduce documentation about how to use and configure the bot
- Recommended Skills: GitHub API, TypeScript/Golang, Webhooks
- Expected project size: Large
- Mentor(s):
  - Ondrej Dubaj (@odubajDT, ondrej.dubaj@dynatrace.com) - primary
  - Florian Bacher (@bacherfl, florian.bacher@dynatrace.com)
- Upstream Issue (URL): https://github.com/keptn/lifecycle-toolkit/issues/2823
- [Create additional metrics operators for KLT](#keptn-additional-metrics)


<a name="keptn-additional-metrics"></a>
### Create additional metrics operators for KLT

Expose additional Observability Platform metrics into K8s as custom metrics

Enhance Keptn Lifecycle Toolkit's metric support by adding four new providers beyond Prometheus 
and Dynatrace and Datadog. This expansion includes both open-source and commercial solutions, 
increasing flexibility and appeal for organizations of diverse sizes.

Outcome:

Metrics and Providers can be specified via CRs
The values for the metrics are stored in the status of the CRs
The metrics adapter is able to fetch these metrics and provide them.

- More info: 
  - https://github.com/keptn/lifecycle-toolkit/issues/525 
  - https://github.com/keptn/lifecycle-toolkit/issues/2850
- Slack channel for technical discussion: `keptn-lifecycle-toolkit-dev`
- Areas to study/improve: Golang, observability, Kubernetes
- Project size: 175 hours

