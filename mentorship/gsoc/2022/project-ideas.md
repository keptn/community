# GSoC Project Ideas - Keptn

Below you can find Google Summer of Code project ideas
which have been proposed for this year by Keptn contributors.
You can find the application guidelines and more information about Keptn i
in GSoC on [this page](../README.md)

## 2022 Project Ideas

> :warning: Full list and more details are coming soon!

### GitOps for Keptn

The configuration of a Keptn project requires a lot of imperative commands, executed in the right order.


The idea is to extend the current Keptn and Keptn GitOps  operators for more management use-cases
based on the prototypes created as a part of the Enhancement Proposal.
Particular details are tio be discussed in the project chat with potential mentors.

- More info: [KEP-67 - Keptn and GitOps](https://github.com/keptn/enhancement-proposals/pull/67)
- Areas to study/improve: Golang, Kubernetes, Operators, Configuration Management
- Potential mentor(s): Oleg Nenashev, Thomas Schuetz

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

### Better GitHub Integration in Keptn

It would be great to provide deeper integration between Keptn and GitHub.
Use-cases: GitHub App Authentication, Reporting to Checks and Deployment API, GitHub Actions executor service.

- Areas to study/improve: Golang, GitHub API
- Potential mentor(s): Oleg Nenashev

### Integration service for k6

[k6](https://k6.io/) is a modern cloud natiove tool for performance testing.
It would be nice to support it as a part of Keptn Quality Gates,
similar to the existing JMeter or Lithmus Chaos services.

- Areas to study/improve: Golang, k6, performance testing
- Potential mentor(s): TBD
 
### Jenkinsfile Executor Service for Keptn
  
The idea is to create a new service that would support executing Jenkins Pipelines as a service in Keptn.
This service would be based on [Jenkinsfile Runner](https://github.com/jenkinsci/jenkinsfile-runner)

- Areas to study/improve: Golang, Java, Jenkins
- Potential mentor(s): Oleg Nenashev

