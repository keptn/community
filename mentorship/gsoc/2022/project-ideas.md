# GSoC Project Ideas - Keptn

Below you can find Google Summer of Code project ideas
which have been proposed for this year by Keptn contributors.
You can find the application guidelines and more information about Keptn i
in GSoC on [this page](../README.md)

## 2022 Project Ideas

- [GitOps for Keptn](#keptn-gitops) 
- [Keptn Plugin for Backstage](#keptn-backstage-plugin)
- [Improve GitHub Integration in Keptn](#keptn-github-integration)
- [Integration Service for k6](#keptn-k6-integration)
- [Jenkins Pipeline Executor Service](#keptn-jenkins-integration)

<a name="keptn-gitops"></a>
### GitOps for Keptn

The configuration of a Keptn project requires a lot of imperative commands, executed in the right order.


The idea is to extend the current Keptn and Keptn GitOps  operators for more management use-cases
based on the prototypes created as a part of the Enhancement Proposal.
Particular details are tio be discussed in the project chat with potential mentors.

- More info: [KEP-67 - Keptn and GitOps](https://github.com/keptn/enhancement-proposals/pull/67)
- Areas to study/improve: Golang, Kubernetes, Operators, Configuration Management
- Potential mentor(s): Thomas Schuetz, Oleg Nenashev

<a name="keptn-backstage-plugin"></a>
### Keptn Plugin for Backstage

[Backstage](https://backstage.io/) is an open platform for building developer portals. 
As the website states, "powered by a centralized software catalog,
Backstage restores order to your infrastructure and enables your product teams
to ship high-quality code quickly — without compromising autonomy".
It would be nice if it was possible to provide Keptn integration for this portal
so that Keptn could be connected as many other tools. See all [Backstage Plugins](https://backstage.io/plugins).

A Possible solution could be a specialized plugin for Keptn using Keptn REST API and/or CLI.
It might be also possible to create a unified plugin for Keptn and other CI/CD tools, 
e.g. implemented on the top of the Cloud Events / CDEvents standard. 


- More info: https://github.com/keptn/keptn/issues/6407 
- Areas to study/improve: Golang, JavaScript, React, Backstage

- Potential mentor(s): Oleg Nenashev, Dmitry Meytin

<a name="keptn-github-integration"></a>
### Improve GitHub Integration in Keptn

GitHub is widely used in proprietary and open source projects.
Currently provides several GitHub Actions that could be used to interact with Keptn:
[sending events to Keptn](https://github.com/keptn/gh-action-send-event) or
[installing Keptn on a GKE cluster](https://github.com/keptn/gh-action-ci-prepare-keptn-cluster),
It would be great to provide deeper integration between Keptn and GitHub,
especially to provide better user experience for users.

Potential use-cases that could be addressed in the project:

-  **GitHub App Authentication Service** with support for executing GitHub REST API calls with GitHub App authentication.
   It is required for accessing GitHub's [Checks API](https://docs.github.com/en/rest/reference/checks) and 
   [Deployments API](https://docs.github.com/en/rest/reference/deployments)
-  **Support for triggering GitHub Actions** from Keptn so that it can invoke GitHub actions from its sequences and auto-remediation steps.
   See [Keptn Issue #2670](https://github.com/keptn/keptn/issues/2670) for more details.
-  **Reporting application statuses to and Deployments API**.
   It would be nice if Keptn could report deployment statuses to GitHub when performing Deployment and auto-remediation sequences.
-  **Reporting Serview Level Objectives(SLOs) and quality gate evaluation results to Checks API**.
   If Keptn quality gate evaluation is triggered from a GitHub branch/pull request (e.g. staging or preview environment deployment in GitHub Actions based CI/CD),
   it would be nice if Keptn coud reportevaluation summaries to [Checks API](https://docs.github.com/en/rest/reference/checks) 

Summary:

- Areas to study/improve: Golang, GitHub API, JavaScript
- Potential mentor(s): Oleg Nenashev

<a name="keptn-k6-integration"></a>
### Integration service for k6

[k6](https://k6.io/) is a modern cloud natiove tool for performance testing.
It would be nice to support it as a part of Keptn Quality Gates,
similar to the existing JMeter or Lithmus Chaos services.

- Areas to study/improve: Golang, k6, performance testing
- Potential mentor(s): TBD
 
 <a name="keptn-jenkins-integration"></a>
### Jenkins Pipeline Executor Service

Jenkins is widely use as a CI/CD automation tool.
It integrates with Keptn through [Jenkins Pipeline Library for Keptn](https://github.com/keptn-sandbox/keptn-jenkins-library) or
through the [CloudEvents Plugin for Jenkins](https://plugins.jenkins.io/cloudevents/).
It is also possible to trigger Jenkins REST APIs from the Job Executor Service.
At the same time it would be great to have deeper integrations with Jenkins as a Pipeline Engine.

Potential deliverables:

* New service that would support executing Jenkins Pipelines on a remote Jenkins instance.
  This service could also wait for completion and extract the executor results from there.
* Executing Jenkins Pipelines right within Keptn's execution plane so that there is no remote Jenkins instance.
  This feature would be based on [Jenkinsfile Runner](https://github.com/jenkinsci/jenkinsfile-runner).

Summary:

- Areas to study/improve: Golang, Java, Jenkins, Jenkins Pipelines
- Potential mentor(s): Oleg Nenashev
