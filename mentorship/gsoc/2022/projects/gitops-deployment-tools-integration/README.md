GSoC 2022 - Integration for GitOps-based Deployment Tools (e.g. ArgoCD/Flux)
==========

To be able to use GitOps tools in combination with Keptn.
The main goal of this project is to find a proper way how the tools could interact with Keptn and to build an integration for such tools.

Deployment tools can be integrated via the helm-service or via the job-executor service.

Currently, there’s no way to integrate GitOps Tools in Keptn. Provide a way such that such tools can be integrated into Keptn return deployment states after the state has been synced.

This project would be done in collaboration with Flux and Keptn maintainers.

## Project team

<!-- TODO: add GitHub and social media links here -->

- Contributor: Meha Bhalodiya - [GitHub](https://github.com/mehabhalodiya) | [LinkedIn](https://www.linkedin.com/in/meha-bhalodiya) | [Twitter](https://twitter.com/mehabhalodiya)
- Mentors:
Thomas Schuetz,
Brad McCoy

## Contacts

- Slack: `#wg-keptn-gitops-operator` on [Keptn Slack](https://keptn.sh/community/#slack)

## Details

As adopters of Keptn move to a GitOps paradigm in their organization it is essential that for the deployment purpose they use Argo/Flux by integrating it in the [keptn/keptn](https://github.com/keptn/keptn) workflow.

As a project that is about to be incubated into the CNCF, it is even more important now to make adoption as seamless as possible. One thing which also might be stated is that many people like to use Argo/Flux and it would bring a huge benefit to the ecosystem when keptn as an orchestrator could deal with this.

The main benefits of integrating this would be that tooling would get changeable. For instance, you can change from Argo to Flux without changing your
testing strategy. Furthermore, it would allow users to use keptn without touching their current deployment tooling.

## References

* [Project page at GSoC website](https://summerofcode.withgoogle.com/programs/2022/projects/yHHRfVz2)
* [Project repository](https://github.com/keptn-sandbox/keptn-flux-integration)
* [Contributor repository](https://github.com/mehabhalodiya/GSoC-22) 
