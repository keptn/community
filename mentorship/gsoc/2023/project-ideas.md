# GSoC Project Ideas - Keptn

This document presents Google Summer of Code project ideas
which Keptn contributors have proposed for this year.
Application guidelines and more information about Keptn
in GSoC are available on [this page](../README.md)

## 2023 Project Ideas

- [Keptn Plugin for Backstage](#keptn-backstage-plugin)
- [Create additional metrics operators for KLT](#keptn-additional-metrics)
- [Revamp the content and the aesthetics of the keptn.sh website](#keptn-website)

<a name="keptn-backstage-plugin"></a>
### Keptn Plugin for Backstage

[Backstage](https://backstage.io/) is an open platform for building developer portals. 
As the website states, "powered by a centralized software catalog,
Backstage restores order to your infrastructure and enables your product teams
to ship high-quality code quickly — without compromising autonomy".
It would be nice to provide Keptn integration for this portal
so that Keptn can connect as many as other tools. See all [Backstage Plugins](https://backstage.io/plugins).

A Possible solution could be a specialized plugin for Keptn using Keptn REST API and/or CLI.
It might be also possible to create a unified plugin for Keptn and other CI/CD tools, 
e.g. implemented on the top of the Cloud Events / CDEvents standard. 

- More info: https://github.com/keptn/keptn/issues/6407 
- Slack channel for technical discussion: `#wg-backstage-integrations`
- Areas to study/improve: Golang, JavaScript, React, Backstage
- Project size: 175 hours
- Potential mentor(s): Brad McCoy

<a name="keptn-additional-metrics"></a>
### Create additional metrics operators for KLT

Expose additional Observability Platform metrics into K8s as custom metrics

This idea consists of two components, a metrics-operator, and a metrics-adapter. The metrics operator manages CRDs for Metrics and Providers, similar to the approach we used in evaluations. The adapter can query these metrics and present them via the Kubernetes Metrics API.

Outcome:

Metrics and Providers can be specified via CRs
The values for the metrics are stored in the status of the CRs
The metrics adapter is able to fetch these metrics and provide them
Limitations:

Currently, this approach seems to work only in a namespaced way, therefore metrics have to be provided per namespace (not sure about specifying them on a cluster level)
There is no history of the metrics available
Further options:

We could define an SLO resource that utilizes metrics
As this provides a very simple, unified way to present metrics in Kubernetes, we could also provide plugins for Argo and Flagger to query the resources
Keptn Evaluations could also use these metrics

- More info: https://github.com/keptn/lifecycle-toolkit/issues/525 
- Slack channel for technical discussion: `#keptn-integrations`
- Areas to study/improve: Golang, observability, Kubernetes
- Project size: 175 hours
- Potential mentor(s): Thomas Schuetz

<a name="keptn-website"></a>
### Revamp the content and the aesthetics of the keptn.sh website

Much of the content on the keptn.sh landing page has been unchanged for a while and needs to be updated to better reflect current projects, themes, and resources.

The look-and-feel of the page should be modernized.
Improve navigation throughout the site. For example, the KLT docs should have the same tabs at the top of the page as the Keptn V1 pages (currently, once you go to the KLT docs, you do not have a path back to the landing page or the Keptn V1 docs).
Make it so the contents in the left frame of content pages remains visible even when the user scrolls down a long page
Add a "Return to top" button for long content pages
Implement CLA to replace DCO and make it easier to contribute to the project.
Once CLA is implemented, add an "Improve this page" link to the displayed docs that pops the user into the github editor for the page and allows them to easily make simple edits and submit them as PRs that can be reviewed and merged.
Point to "Resources" that are current and implement a scheme that makes it easier to update those listings
Consider whether the Tutorials link on the
Consider a "banner" or some similar scheme that makes it easier to post current news and information, such as upcoming conferences, hackathons, et cetera

- More info: https://github.com/keptn/lifecycle-toolkit/issues/743
- Slack channel for technical discussion: `#keptn-integrations`
- Areas to study/improve: Frontend
- Project size: 175 hours
- Potential mentor(s): Meg McRoberts
