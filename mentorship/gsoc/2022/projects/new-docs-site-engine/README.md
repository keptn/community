# GSoC 2022 - New Documentation Site Engine

This project is about a New Documentation Site Engine for Keptn which can handle a large number of documentation projects of Keptn. Currently, the Keptn documentation site is based on Hugo based theme called `hugo-serif-theme`. For tutorials, _Codelabs_ is also used. While extremely handy for smaller projects and initial versions of Keptn, this toolchain has serious deficiencies for larger-scale projects like Keptn.

The new Documentation Site engine will be based on Docusaurus. Docusaurus is an optimized site generator in React. Docusaurus helps you to move fast and write content. Build documentation websites, blogs, marketing pages, and more. The main focus of Keptn New Documentation Site Engine will be managing large-scale documentation and complex documentation projects. So two major things which are needed in the documentation engine are the ability to build the documentation from the source located in multiple repositories and support for document versioning.

## Project team

- Contributor: Rajiv Ranjan Singh
- Mentors: Indermohan Singh, Meg McRoberts, Suraj Banakar

## Contacts

- Slack: `#keptn-docs` on [Keptn Slack](https://keptn.sh/community/#slack)

## Details

#### Project scope & deliverables

The user docs site is designed to assist end-users in using a product or service. The excellent user docs site is significant because it provides an avenue for users to learn how to use the software, its features, tips, and tricks, and resolve common problems encountered when using the software. It also reduces support costs and is part of the corporate identity of the product. The excellent user docs site is a sign of the healthiness of the product, and the developer team. Without a good user docs site, a user may not know how to do the above things effectively and efficiently. User docs site can play a pivotal role in ensuring a product's success because excellent communication is and will always be at the heart of any business or development. Fantastic documentation takes that communication and puts it in a manageable framework that everyone can access for success.

#### Expected Deliverables

- Support for the latest link pointing to the documentation for the last release.
- Use versioned documentation from external sources, ideally from version tags and branches.
- Move documentation sources to code repositories so that we could enable documentation as code and make documentation patches a part of the contribution process.
- Automation that builds the site from multiple repositories. It includes scripting, GitHub Actions, and automated configuration management.
- GitHub workflows for continuous deployment of the website to GitHub Pages, Netlify, Vercel, etc.
- Implement previews for the website and support for staging changes (e.g. pre-release documentation). Developer and Contributor documentation for the new engine, in collaboration with the documentation contributors.

and many more.

#### Future work based on Project

After completion of the above deliverables, we can work on the following:

- Improving SEO of versioned docs and the whole documentation site.
- Adding interactive documentation example by rendering JSX in markdown content with the help of MDX support of Docusaurus.
- Adding standalone Pages for a great user experience.
- Improving UI of the documentation site.

and many more.

## References

- [Contributor GSoC 2022 repository](https://github.com/iamrajiv/GSoC-2022)
- [Detailed GSoC 2022 Project Proposal](https://github.com/iamrajiv/GSoC-2022/blob/main/GSoC_2022_Project_Proposal.md)
- [Project page at GSoC 2022 website](https://summerofcode.withgoogle.com/programs/2022/projects/whEHkPZx)
- [Project timeline & issues](https://github.com/keptn-sandbox/new-keptn-docs-engine/projects/1)
