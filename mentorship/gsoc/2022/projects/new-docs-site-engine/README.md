<div align="center">
<img src="https://raw.githubusercontent.com/iamrajiv/GSoC-2022/main/assets/gsoc-2022-1.svg" height="auto" width="600" />
<br />
<img src="https://raw.githubusercontent.com/iamrajiv/GSoC-2022/main/assets/gsoc-2022-2.svg" height= "auto" width="400" />
<br />
<h1>Keptn</h1>
<h3>
New Documentation Site Engine
</h3>
</div>

## Table of Contents

- [Introduction](#introduction)
- [Project team](#project-team)
- [Contacts](#contacts)
- [Problem Statement](#problem-statement)
- [Work Summary](#work-summary)
  - [Phase 1](#phase-1)
  - [Phase 2](#phase-2)
  - [Miscellaneous Phase](#miscellaneous-phase)
- [Future Work to be done](#future-work-to-be-done)
- [Meetings Details](#meetings-details)
- [Challenges Faced](#challenges-faced)
- [Learnings](#learnings)
- [Acknowledgments](#acknowledgments)
- [References](#references)

## Introduction

This project is about a New Documentation Site Engine for Keptn which can handle a large number of documentation projects of Keptn. Currently, the Keptn documentation site is based on a [Hugo](https://gohugo.io/) theme called [hugo-serif-theme](https://github.com/zerostaticthemes/hugo-serif-theme). For tutorials, [Codelabs](https://github.com/googlecodelabs/tools) is also used. While extremely handy for smaller projects and initial versions of Keptn, this toolchain has serious deficiencies for larger-scale projects like Keptn.

The new Documentation Site engine will be based on Docusaurus. Docusaurus is an optimized site generator in React. Docusaurus helps you to move fast and write content. Build documentation websites, blogs, marketing pages, and more. The main focus of Keptn New Documentation Site Engine will be managing large-scale documentation and complex documentation projects. So two major things which are needed in the documentation engine are the ability to build the documentation from the source located in multiple repositories and support for document versioning.

Keptn is an event-driven orchestration engine for cloud-native apps. Started in 2018, it uses a declarative approach to automate delivery and operations so they can be scaled up to a large number of services. Keptn evaluates _Service Level Indicators (SLOs)_ and provides a dashboard, alerts, and auto-remediation for them. It also provides integrations with the Cloud Native ecosystem including _Prometheus_, _ArgoCD_, _CloudEvents_, _Backstage_, and many other cloud-native projects.

## Project team

- Contributor: [Rajiv Ranjan Singh](https://github.com/iamrajiv)
- Mentors: [Indermohan Singh](https://github.com/imsingh), [Meg McRoberts](https://github.com/StackScribe), [Suraj Banakar](https://github.com/vadasambar)

## Contacts

All documentation-related discussions are done in the [#keptn-docs](https://keptn.slack.com/archives/C017T4KUAG3) channel on the Keptn Slack workspace.

## Problem Statement

Making a **New Documentation Site Engine** for Keptn which can handle a large number of documentation projects of Keptn.

**Open Issue:** [https://github.com/keptn/keptn.github.io/issues/994](https://github.com/keptn/keptn.github.io/issues/994)

**Project Idea:** [https://github.com/keptn/community/blob/main/mentorship/gsoc/2022/project-ideas.md#new-documentation-site-engine](https://github.com/keptn/community/blob/main/mentorship/gsoc/2022/project-ideas.md#new-documentation-site-engine)

## Work Summary

I had divided the Development Phase into two phases i.e. `Phase 1` and `Phase 2`.

> `Phase 1` was to deal mostly with implementing core features and functionality needed in the documentation engine.

> `Phase 2` was to deal mostly with implementing miscellaneous features and functionality of the documentation engine like Continuous Integration, Continuous Deployment, etc.

#### Phase 1

> **Week 1 - Week 6 (June 13 - July 25, 2022)**

---

- [x] Initialization and deployment of the documentation engine based on Docusaurus from scratch.

  - [x] Initialised the new Docusaurus site using `npx create-docusaurus@latest new-keptn-docs-engine classic` command and push the changes to [keptn-sandbox/new-keptn-docs-engine](https://github.com/keptn-sandbox/new-keptn-docs-engine).

    > Above task is done and I have pushed the changes directly to the repository. Commit can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/commit/e2f2202b01894806e1d9e924d97abb2b98b2d8d1](https://github.com/keptn-sandbox/new-keptn-docs-engine/commit/e2f2202b01894806e1d9e924d97abb2b98b2d8d1).

  - [x] Adding as basic documentation on how to use Docusaurus and what configuration of Docusaurus we are following like Project structure, Templates, etc.

    > I used the `npx create-docusaurus@latest new-keptn-docs-engine classic` command to create the new Docusaurus site so in this case, I used the `classic` template. Docusaurus recommend the `classic` template so that we can get started quickly, and it contains features found in Docusaurus 1. The `classic` template contains `@docusaurus/preset-classic` which includes standard documentation, a blog, custom pages, and a CSS framework (with dark mode support). We can get up and running extremely quickly with the classic template and customize things later on when you have gained more familiarity with Docusaurus. We can also use the template's TypeScript variant by passing the `--typescript` flag. See [TypeScript support](https://docusaurus.io/docs/typescript-support) for more information.

  - [x] Deploying the new Docusaurus site engine to Netlify.

    > [https://github.com/keptn-sandbox/new-keptn-docs-engine](https://github.com/keptn-sandbox/new-keptn-docs-engine) has been deployed to Netlify at [https://keptn-experimental-docs-site.netlify.app/](https://keptn-experimental-docs-site.netlify.app/).

  - [x] Adding `CONTRIBUTING.md` file with content related to how to add contents in Docusaurus and how to use it concerning Keptn. Also, this work will go on since we will be adding more content in the future according to documentation needs.

    > PR related to adding `CONTRIBUTING.md` file is [https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/4](https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/4).

Issue link: [https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/2](https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/2)

---

- [x] Adding UI and UX changes, moving the content and search functionality to the new documentation site engine.

  - [x] Implementing UI and UX changes in the documentation engine like creating components, templates, standalone pages, etc.

    > Created the new components, templates, standalone pages, etc for the documentation engine. I had refactored the default components and templates of the Docusaurus site which were added when the Docusaurus site was initialized.

    > Above task is done and I have pushed the changes directly to the repository. Commit can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/commit/b749bbdfebfeaa41c789cd4c91ac29032ac1bbfa](https://github.com/keptn-sandbox/new-keptn-docs-engine/commit/b749bbdfebfeaa41c789cd4c91ac29032ac1bbfa).

    > After getting feedback from mentors on the new documentation site engine, I have refactored the documentation engine. PR can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/9](https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/9).

  - [x] Finalizing the things that need to be copied from the current documentation engine to the new documentation site engine with proper structure.

  - [x] Copying content from the current documentation engine to the new documentation site engine which has been finalized.

    > As of now not all contents are copied from the current documentation engine to the new documentation site engine instead, some documents are copied to the new documentation site engine.

  - [x] Adding documentation search functionality.

    > As of now I have added local search support using a [docusaurus-lunr-search](https://github.com/praveenn77/docusaurus-lunr-search) local search plugin but in the future, we can update this to [Algolia DocSearch](https://docsearch.algolia.com/).

    > Adding Algolia DocSearch support to the documentation engine is not part of this proposal but it is a suggestion to add it in the future.

    > PR related to adding documentation search functionality can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/11](https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/11).

Issue link: [https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/5](https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/5)

---

- [x] Adding Versioning of docs support feature.

In current docs, we don't have versioning of docs support feature. As of now, we were versioning the docs manually. To solve this problem we have added versioning of the docs support feature using Docusaurus. We can use the versioning CLI to create a new documentation version based on the latest content in the `docs` directory. That specific set of documentation will then be preserved and accessible even as the documentation in the `docs` directory continues to evolve.

> PR related to adding versioning support can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/10](https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/10).

---

- [ ] Adding Multiple repository docs support feature.

This feature is partially done and we want more clarity on this feature. Earlier we thought adding Docusaurus Multi-instance support will solve this problem but it is not the case. The thing is using Docusaurus Multi-instance we can have multiple `docs` folders in the same Docusaurus site and for every `docs` folder, we can put our documentation accordingly. But we wanted something automatic stuff so that we can pull docs from other repository and organize it in these `docs` folder instances.

I got clarity about this feature a little late so I was not able to implement this feature completely.

Some reasons why we want the Multiple repository docs support feature:

- Keptn CLI docs are generated using the `keptn generate docs` command. As of now, we run it in GitHub action [here](https://github.com/keptn/keptn.github.io/blob/9c649b434c9081028e0cc3535c9fa3a4217941fb/.github/workflows/auto-update.yml#L72) to populate our docs repo with CLI docs.
- If we look at the architecture doc [here](https://keptn.sh/docs/concepts/architecture/), the Keptn control plan consists of multiple services which have their READMEs in the main Keptn repository ([example](https://github.com/keptn/keptn/tree/master/jmeter-service)). Just look for any directory with `service` in [https://github.com/keptn/keptn](https://github.com/keptn/keptn), we can see individual READMEs for all such services. It's a good idea to move these READMEs to the docs site because the people who develop and maintain these services are responsible for updating the READMEs. Having them in a single place just makes it easier to update the READMEs and read them later as well.
- We also have services that extend the control plane which sits in a separate repository. Check [dynatrace-service](https://github.com/keptn-contrib/dynatrace-service) for example. As of now, if we add a new service that extends the control plane, we also have to add some documentation around it manually in the main docs repository.
- We have a miscellaneous repository like [Keptn spec](https://github.com/keptn/spec), documentation around what different values mean in the Keptn helm chart which we can't put in the main docs repository because they serve a different purpose.

  - [x] Adding Docusaurus Multi-instance support.

    > PR related to adding Docusaurus Multi-instance support can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/12](https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/12).

  - [ ] Adding GitHub Action that can pull the docs from multiple repositories.

> We want a GitHub Action which can pull the docs from [https://github.com/keptn/keptn.github.io](https://github.com/keptn/keptn.github.io) to [https://github.com/keptn-sandbox/new-keptn-docs-engine](https://github.com/keptn-sandbox/new-keptn-docs-engine) repository and organize the docs accordingly. Also, we are not sure this is the right approach to solve this problem. But it's one of the approaches we have thought of.

---

#### Phase 2

> **Week 7 - Week 12 (July 26 - September 5, 2022)**

---

- [x] Integrating [Lighthouse](https://developers.google.com/web/tools/lighthouse) CI.

Every webpage that is crawled by a search engine is evaluated with a score from 5 categories: Performance, Accessibility, Best Practices, SEO, and PWA. This is given a score between 0 – 100. The better your lighthouse score will affect how high up your webpage will appear on a search engine.

With a high score, your site meets the best practices and SEO standards outlined by Google in terms of performance and accessibility. Lighthouse is an important tool because it can identify common problems that affect the quality of your websites and propose solutions for them.

Lighthouse CI is a suite of tools that make continuously running, saving, retrieving, and asserting against [Lighthouse](https://github.com/GoogleChrome/lighthouse) results as easily as possible. So we have integrated Lighthouse CI GitHub Action into the new documentation site engine.

> PR related to adding Lighthouse CI can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/17](https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/17).

Issue link: [https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/16](https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/16)

---

- [x] Adding [Vale](https://github.com/errata-ai/vale) linter for doc quality checks.

To solve problems related to the styling of documentation, linting, doc quality checks, etc we wanted some tool to achieve these things.

We research and found [proselint](https://github.com/amperser/proselint) and [Vale](https://github.com/errata-ai) which can full fill our needs. After going through both we feel Vale has a lot of features as compared to `proselint` and is widely used in many popular open source organizations.

So, we integrated [vale-action](https://github.com/errata-ai/vale-action) in the new documentation site engine.

Also, for the time being, I have adopted the [Google Style Guide](https://google.github.io/styleguide/) because my main motivation is to integrate the Vale GitHub Action into the docs engine. Yeah, I think we can have a separate discussion about which style guide to follow or we can have our custom style guide as well.

One of the limitations of Vale is that we have to update things in `vocab.txt` which is required for false positives. Some keywords, and names (e.g. `Keptn`, `KEP` etc) are considered as `vale.Spelling` errors, so we have to add them inside `vocab.txt` file. We can list all unique words which are considered errors in `vocab.txt` using the below command.

```shell
yarn run lint:docs | grep -o "'[a-z A-Z]*'" | grep -o "[a-z A-Z]*" | sort | uniq > .github/styles/vocab.txt
```

Now we have to manually validate all words listed in `vocab.txt`, discard which are invalid and correct them in the file where they were located.

Now we have to manually validate all words listed in `vocab.txt`, discard which are invalid and correct them in the file where they were located.

> PR related to adding Vale linter can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/19](https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/19)

Issue link: [https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/19](https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/19)

---

- [x] Adding [Prettier](https://prettier.io/) GitHub Action support to format docs.

[Prettier](https://prettier.io/) is a very popular code formatter that uses very opinionated but sensible styles to format your code and prevent ongoing debates about code styles. So we wanted a GitHub action to automatically format your code using Prettier.

To set up the GitHub action, all we need to do is install our dependencies (e.g. `yarn install`), run our format script (e.g. `yarn format`), and then commit any changes if necessary.

By utilizing Prettier with GitHub Actions, we can ensure that our code is formatted consistently and without any issues.
It also helps to reduce manual work when formatting code.

> PR related to adding Prettier GitHub Action can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/25](https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/25)

Issue link: [https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/23](https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/23)

---

- [x] Adding GitHub Action to check broken links in docs.

It is a GitHub Action that can be run on the docs to check for broken links and xrefs. The GitHub Action can create an issue on the repository with the broken links report, add labels to the issue and assign it to the relevant maintainers.

> PR related to adding GitHub Action to check broken links in docs can be found here [https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/28](https://github.com/keptn-sandbox/new-keptn-docs-engine/pull/28)

Issue link: [https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/27](https://github.com/keptn-sandbox/new-keptn-docs-engine/issues/27)

---

- [x] Finalizing the project deliverables and refactoring the code if any, based on the feedback.
- [x] Making the project report and requesting mentors to review the project report.
- [x] Finalizing and submitting the project report and other related documents.

---

#### Miscellaneous Phase

**NOTE:** Multiple repository docs support feature is not yet implemented completely and it is still in progress. As of now `Docs Multi-instance` support is added which is a`@docusaurus/plugin-content-docs` plugin. Adding GitHub Action which can pull the docs from multiple repositories is not yet implemented.

- Adding internationalization ([i18n](https://en.wikipedia.org/wiki/Internationalization_and_localization)) support. A possible translation strategy is to version control the translation files with Git (or any other VCS).

  > Discussion on this is done [here](https://keptn.slack.com/archives/C017T4KUAG3/p1657235519862879) and we have put this on lower priority.

- Implementing all SEO approaches listed in [https://docusaurus.io/docs/seo](https://docusaurus.io/docs/seo) like adding metadata in site configuration, adding metadata for all single pages, adding metadata in the front matter of all markdown files, etc.

  > This will take some time to implement as we will be adding metadata in the front matter of all files and will be implementing slowly as we still moving the content to the new documentation site engine.

## Future Work to be done

These are work that was part of this proposal but was partially implemented or not implemented at all like:

- Adding Multiple repository docs support feature.

  > This is an important feature which we have to implement in the future. We have to implement this feature in such a way that we can add multiple repositories docs in the same documentation engine. This will help us to have a single documentation engine for all the repositories which we want to have in the documentation engine.

- Adding internationalization ([i18n](https://en.wikipedia.org/wiki/Internationalization_and_localization)) support.

  > This work is a part of the miscellaneous phase. Discussion on this is done [here](https://keptn.slack.com/archives/C017T4KUAG3/p1657235519862879) and we have put this on lower priority.

- Implementing all SEO approaches listed in [https://docusaurus.io/docs/seo](https://docusaurus.io/docs/seo) like adding metadata in site configuration, adding metadata for all single pages, adding metadata in the front matter of all markdown files, etc.

  > This work is a part of the miscellaneous phase. This work was not able to complete because this can only be done when we are fully ready with a plan of what content we are going to have in the documentation engine with proper structure.

Apart from proposal work, we had to do some other work like during my coding phase I got a lot of feedback and suggestions from mentors and other community members. Some small suggestions were implemented and some suggestions were not implemented because of the time constraint.

So, some important work that needs to be done in the future are:

- Making good UI/UX for the new documentation site engine. We have to make sure that the UI/UX of the documentation engine is good and easy to use. We have to make sure that the UI/UX is good for both desktop and mobile devices. We need a discussion on this and we have to make sure that we are following the best practices for UI/UX.
- Migrating the content from the old documentation site engine to the new documentation site engine. Also, we need to have a proper plan about how the docs are going to be structured in the new documentation site engine. Meg has put together a quick list of the structure we should for when we move content from the old documentation site engine to the new documentation site engine. A thread on this can be found [here](https://keptn.slack.com/archives/C017T4KUAG3/p1656741348364249).
- Writing our own custom rules for Vale linter. As of now, we are following the [Google Style Guide](https://google.github.io/styleguide/) for Vale linter.
- Adding Docusaurus component which can render shipyard files. Discussion on this is done [here](https://keptn.slack.com/archives/C017T4KUAG3/p1661899657043279). The GitHub issue can be found [here](https://github.com/keptn/keptn.github.io/issues/1409).

Other than the above work, we can find other suggestions in meeting notes [here](https://github.com/iamrajiv/GSoC-2022/blob/main/GSoC_2022_Meetings.md#8th-august-2022).

## Meetings Details

All the meeting notes can be found [here](https://github.com/iamrajiv/GSoC-2022/blob/main/GSoC_2022_Meetings.md).

## Challenges Faced

The most challenging part was the `Adding Multiple repository docs support feature` but I have implemented it partially. Also, the project requirement was not so clear I was not sure whether the migration of content from the old documentation site engine to the new documentation site engine is part of the project or not. Scheduling meetings like mentors and mentees were at different time zones so it was a little bit hard to sync up but we did it and we had a great meeting.

## Learnings

I am very glad that I had the opportunity to take part in the Google Summer of Code program. Participating in this program has helped me to:

- Proper PoC and understanding are very important before starting the project or any feature and also we should have other alternatives before choosing the best one. This thing I got to learn when the `Adding Multiple repository docs support feature` was not implemented fully because I did not understand the feature properly. The problem with multiple repository docs support was at starting I thought we only need `Docusaurus Multi-instance support` which is the same as hosting multiple docs in a single docusaurus project but after that, I got to know that in addition to `Docusaurus Multi-instance support` we need to pull docs from other repositories and organize it in new documentation site engine. But again I was not sure where to pull docs from whether I have to pull from [https://github.com/keptn/keptn.github.io](https://github.com/keptn/keptn.github.io) repository or multiple repositories and combine and organize all docs to new documentation site engine. I discussed this with my mentors and I got clarity on this. We got to know a lot of ways we can implement this feature. Since it was taking a lot of time so I moved to other work and I thought I will pick this up at last because this work needs a lot of time and research and I was not sure how to implement this feature.
- Learned about Keptn, Docusaurus, GitHub Actions, How to make good PRs, How to make proper commit messages, JavaScript XML(JSX), Keptn CLI, MDX, Writing proper documentation, etc.
- Planning and structuring the requirements for the project and managing high-priority tasks and low-priority tasks.
- How to work in a team and how to communicate with the team.

Apart from the above, I have learned a lot of things from my mentors and other community members. I am very thankful to my mentors and other community members for helping me throughout the program.

## Acknowledgments

I am deeply grateful to my mentors [Indermohan Singh](https://github.com/imsingh), [Meg McRoberts](https://github.com/StackScribe), and [Suraj Banakar](https://github.com/vadasambar), who guided me patiently through the project and were always ready to help, review work in progress, gave feedback regarding the overall shape of the project and the feasibility of certain solutions and maintained a very friendly, supportive, and stimulating atmosphere on the team. They devoted a lot of time to this project and led the video meetings in a well-organized, yet non-stressful manner. Their support and positivity helped me through this project and made me enjoy every bit of it. I would also like to thank [Moritz Wiesinger](https://github.com/mowies), [Oleg Nenashev](https://github.com/oleg-nenashev), and other keptn community members for their support and feedback. Last but not least, I would like to thank Google and Google Summer of Code organizers for this initiative.

## References

- [Contributor GSoC 2022 repository](https://github.com/iamrajiv/GSoC-2022)
- [Contributor Proposal link](https://summerofcode.withgoogle.com/media/user/f68762051013/proposal/gAAAAABjGvyZjqW5uiTvSpQ-s46PD6X5k6KtZzJ-9x-PSrVRbNh-4k_mTfVrlZgMKJ7iLBYynUjHJ2pahKD4Su86Xch-Caej8cdp7MOQh5JHHXpiNsoTZDk=.pdf)
- [Doc Tools Requirements](https://docs.google.com/document/d/1VvDtVW-zV8bfhHNrXBNZdJz5s81a1M1eulov8_ahqo0/edit#heading=h.fyeyfl7x8jho)
- [GitHub Project board](https://github.com/keptn-sandbox/new-keptn-docs-engine/projects/1)
- [https://github.com/iamrajiv/keptn-docusaurus-poc](https://github.com/iamrajiv/keptn-docusaurus-poc)
- [https://github.com/keptn](https://github.com/keptn)
- [https://keptn-docusaurus-poc.vercel.app/](https://keptn-docusaurus-poc.vercel.app/)
- [https://keptn.sh/](https://keptn.sh/)
- [Meetings](https://docs.google.com/document/d/1pgI0XW3T9wIix70OZsQ2F-9cGtLmXH1jkyhXm4v-RV0/edit#heading=h.xbcx68nc01mi)
- [New Documentation Site Engine Issue link](https://github.com/keptn/keptn.github.io/issues/994)
- [Project detail at Keptn Community repository](https://github.com/keptn/community/tree/main/mentorship/gsoc/2022/projects/new-docs-site-engine)
- [Project page at GSoC 2022 website](https://summerofcode.withgoogle.com/programs/2022/projects/whEHkPZx)
- [Restructure documentation](https://docs.google.com/document/d/12xVgFSV5Q7keDXOqVFE8pqY0Qkhq--nKsP-7NkVuyjA/edit#heading=h.vm22oe3mkivh)

<div align="right">
<img src="https://raw.githubusercontent.com/iamrajiv/GSoC-2022/main/assets/gsoc-2022-3.svg" height="auto" width="100" />
</div>
