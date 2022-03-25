# Keptn in GSoD 2022 - Project description

This document presents the Google Season of Docs project
which Keptn contributors have proposed for this year.
Application guidelines and more information about Keptn
in GSoD are available on [this page](../README.md).

## 2022 Project. Re-architecting and improving Keptn user documentation

During GSoC 2022 we will run either one large-size project or two small-size ones.
You will work with the static Keptn website and the documentation engine based on the modern technology stack.
Currently we use Hugo for the website and Docs, and Google Codelabs for tutorials.
We plan adoption Docusaurus or Antora as a new documentation platform during Google Summer of Code 2022
([project idea](https://github.com/keptn/community/blob/main/mentorship/gsoc/2022/project-ideas.md#new-documentation-site-engine)).
Technical writers in this project will be able to work with one of these technologies while
using the Documentation-as-Code approach and Mardown/Asccidoc languages.

### Key deliverables

We offer the technical writers to focus on 2-3 deliverables from the list below:

- Installation Guidelines for Keptn and Keptn CLI client on common Kubernetes clusters.
  This deliverable will update or replace the existing documentation.
- New example projects that demonstrate key Keptn capabilities to newcomer users and potential adopters.
  This deliverable will update or replace the existing documentation and tutorials.
- Restructure existing documentation to user and administrator guidelines
  and developer guides.
- Reference pages for key information and concepts that are not specific to Keptn versions.

### Details for each deliverable

#### Installation Guidelines

Create and test installation instructions for creating a k8s cluster on which Keptn can be installed for demo and evaluation purposes.
Create excellent instructions for installing Keptn CLI and Keptn on this new cluster.
Confirm that one set of instructions works for all k8s implementations and all “Keptn curious” projects we provide. 
If necessary, create multiple instruction sets, clearly defining when each is appropriate.

Also, we propose to create and test instructions for installing a Keptn “playground” in an existing k8s cluster for study and demos. 
The goal here is to provide an environment where someone can try Keptn out with their existing data without risking damage to an existing production system (such as Prometheus, Dynatrace, DataDog, etc.)

For this deliverable, instructions should be pedagogical rather than pure cookbook:
provide enough explanation that the user gains some understanding of what they are doing.
Include information for verifying each step and some troubleshooting information or links.

#### New example projects

Create 5-6 projects that introduce key Keptn capabilities for the Keptn curious to explore. 
We have a number of existing tutorials to use as starters or inspiration. 
Note that many of the existing tutorials use the [sockshop project](https://github.com/keptn-demo/sockshop) as a base;
and some updates will be needed there.

Each project should include:

- Files that can be downloaded from github to provide some basic configuration with an explanation of what is provided in these files (that they would have to do themselves if they wanted to implement this functionality.
- Specification in GitHub for what needs to be installed to provide a viable environment for the project, including integrations that must be included, configurations that must be set, and so forth.
- Excellent information about how to run the sample project and do the exercises, including context for each step, what to look for to determine success and understand the output.  The goal is to begin to educate the user about how to get the most out of Keptn

#### Separate guides for roles

We want to introduce separate documentation for different Keptn user roles: 
administrators, end users and developers.
We suggest to work together to regroup the content so that the new structure is introduced.

#### New reference pages

Rewrite reference pages for files to conform to the structure proposed in the [Structure of reference pages](https://docs.google.com/document/d/1rmSGUFsnYuNc_BGHGmkW-9iB3hrOYbMeA-mJmMOjGRk/edit?usp=sharing) proposal.
We are currently creating reference pages for critical files by capturing information in existing doc files, source code README files, etc.
This project would be to restructure and expand the information in these files to create proper reference pages.
It might also include relocating some information in existing files to a more appropriate location.

Same for other standard documentation independent from version.
Set a standard for what information belongs in a “Concepts” article versus
what belongs in reference pages or guides that are currently
located in the version-specific sections of the documentation.
Then modify the existing Concepts articles to conform to this standard and create Concepts articles for appropriate concepts that
are discussed in existing guides or elsewhere
(such as README files in the software repos or existing Keptn videos).

Creating missing guides is not part of this project

## Alternative project ideas

We also discussed a number of alternative project ideas that can be considered.

### Documentation assessment

This project would assess the Keptn documentation, to help us come with a plan for improving our documentation. In particular, we're looking for someone to look at the content organization, the clarity of the language and concepts, and to make sure it's as readable as possible for both implementors and end users.

- More info: [tech docs](https://github.com/cncf/techdocs/blob/main/assessments/howto.md) and [criteria](https://github.com/cncf/techdocs/blob/main/assessments/criteria.md)
- Slack channel for technical discussion: `#keptn-docs`
- Areas to study/improve: Technical writing, Documentation, English, Git
- Project size: 
- Difficulty: Easy
- Potential mentor(s): Meg McRoberts

### Restructure contributing documentation

Architect information about how to contribute to Keptn
(and potentially related projects),
get community approval for the proposal, then implement it. 
For some preliminary notes about what is currently there and issues, see
[this proposal](https://docs.google.com/document/d/10rhdsh3E-d4zYq1jJzS6cJM78x1ViyPvRZVkn-h4HgY/edit?usp=sharing).

### More ideas

For ideas that didn't make to this list,
see [this document](https://docs.google.com/document/d/154zrnkUdUhyWyDB-Gs123JvbiYPb-zQDLaV2Oe0PC8A/edit#heading=h.ckoz6t2d3tab).
