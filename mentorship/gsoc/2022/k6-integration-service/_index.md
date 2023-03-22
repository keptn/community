---
title: K6 Integration Service
linktitle: K6 Integration Service
---

<div align="center">
<img data-proofer-ignore src="https://raw.githubusercontent.com/iamrajiv/GSoC-2022/main/assets/gsoc-2022-1.svg" height="auto" width="600" />
<br />
<img data-proofer-ignore src="https://raw.githubusercontent.com/iamrajiv/GSoC-2022/main/assets/gsoc-2022-2.svg" height= "auto" width="400" />
<br />
<h1>Keptn</h1>
<h3>
K6 Integration Service
</h3>
</div>

## Table of Contents

- [Introduction](#introduction)
- [Project team](#project-team)
- [Contacts](#contacts)
- [Work Summary](#work-summary)
  - [Run Standard K6](#run-standard-k6)
  - [Support for K6 extensions](#support-for-k6-extensions)
  - [Quality Gates Evaluation](#quality-gates-evaluation)
  - [Tutorials](#tutorials)
- [Challenges](#challenges)
- [Acknowledgments](#acknowledgments)
- [Project Resources](#project-resources)
- [References](#references)

## Introduction

K6 is an open-source tool widely used for load testing.
With Keptn’s Quality gates, we can automate the process of evaluating the results of the test and also monitor them.
Keptn already supports JMeter, Locust, Litmus Chaos, and others.
This project will enable users to use K6 for performance testing.
Further goals include adding SLI and SLO compliance using Prometheus which K6 supports using Extensions.

## Project team

<!-- TODO: add GitHub and social media links here -->

- Contributor: Jainam Shah - [GitHub](https://github.com/jainammm/) | [LinkedIn](https://www.linkedin.com/in/jainammm/) | [Twitter](https://twitter.com/jvenommm)
- Mentors:
  - Pepe Cano - [GitHub](https://github.com/ppcano/) | [LinkedIn](https://www.linkedin.com/in/ppcano/) | [Twitter](https://twitter.com/ppcano_)
  - Adam Gardner - [GitHub](https://github.com/agardnerit/) | [LinkedIn](https://www.linkedin.com/in/agardner1/)

## Contacts

- Slack: `#wg-k6-integrations` on [Keptn Slack](https://keptn.sh/community/#slack)

## Project Details

Support for K6 will help extend Keptn community users to switch/use it as performance testing tool.
K6 is considered to be a modern tool for DevOps like Keptn, so the community might be inclined towards using it.

Some of the features of K6 include:

- It has good resource utilization and one load generator can simulate tens of thousands of virtual users
- It is code-driven, with JavaScript as scripting language
- K6 has native support for Prometheus

Thresholds in K6 are used for some specific pass/fail criteria. This feature is very commonly used. Based on passed/failed of Thresholds results, we'll return the state to the Keptn control plane.

The K6 service will suscribe to the `sh.keptn.event.test.triggered` CloudEvent and execute the Load Testing. K6 will write the metrics to Prometheus for further step of SLO evaluation.

## Work Summary

The three major milestones of this project were as follows:

1. Run standard K6
2. Support K6 extensions
3. Use the metrics exported by K6 Extension for Keptn's Quality Gate evaluations

All the three milestones were achieved.

### Run Standard K6

For POC, we used the Job Executor Service for running K6 test. Job Executor Service was able to execute tests. The `stdout` logs were shown on Bridge and the task failed/passed based on K6 thresholds pass/fail criteria.

### Support for K6 extensions

For K6 extensions support we stumbled upon the design of implementing a new Keptn service or Job Executor will do the job. Here I wrote a the boilerplate code for new Keptn service. We finally decided to move ahead with the Job Executor Service because making the Docker image and pushing it to registry did the Job. We need the install the supported tool in K8s and reachable from Keptn namespace. Kubernetes secrets and environment support in Job Executor Service helped in K6 extensions execution.

### Quality Gates Evaluation

Once K6 extension support started writing the metrics to Prometheus, Keptn's quality gates were able to fetch the SLI and do compliance check. We can add tags in K6 extension which allows us the indentify the metrics based on project, stage and service. This allows us to have best of both the worlds: K6 thresholds and Keptn Quality Gates

### Tutorials

The tutorials have been kept in 3 parts in the main project repository: [keptn-sandbox/k6-service](https://github.com/keptn-sandbox/k6-service)

## Challenges

Various challenges were faced during the project. Some are

- Job Executor Service and Keptn setup
- Communication from K6 extension running in JES and Prometheus
- Docker images for K6 extension not published officially
- Unique identifier for the K6 metrics in Prometheus based on project, stage and service

## Acknowledgments

I would like to thank [Adam Gardner](https://github.com/agardnerit/) and [Pepe Cano](https://github.com/ppcano/) for mentoring me through the GSOC period and helping me learn lot of cool things. I'd also like to thank [Oleg Nenashev](https://github.com/oleg-nenashev) and [Keptn](https://github.com/keptn/keptn) Community for providing me this opportunity.

## Project Resources

- [Repository](https://github.com/keptn-sandbox/k6-service)
- [SCRUM Board](https://github.com/keptn-sandbox/k6-service/projects/1)
- [Meeting Minutes](https://docs.google.com/document/d/1A3gbtQ6-YOTpO3v_ltBgHWTODFt93zByHXWVJ6r0jcg/edit?usp=sharing)

<!-- * Meeting Schedule [No Longer Scheduled]
  * Every Thursday @ 8:30 UTC
  * [Zoom Link](https://dynatrace.zoom.us/j/96378132758?pwd=Z0NRbXhxNlJiSjRqMkd5cmlLWEJMUT09) -->

## References

- [Project page at GSoC website](https://summerofcode.withgoogle.com/programs/2022/projects/0xICJhw8)
- [Contributor Proposal Link](https://docs.google.com/document/d/1wG8Mobj5Hpa6x82KN7VdXqDwC_kBEHes/edit?usp=sharing&ouid=110707808117776486784&rtpof=true&sd=true)
- [https://github.com/keptn](https://github.com/keptn)
- [https://github.com/grafana/k6](https://github.com/grafana/k6)

<div align="right">
<img src="https://raw.githubusercontent.com/iamrajiv/GSoC-2022/main/assets/gsoc-2022-3.svg" height="auto" width="100" data-proofer-ignore/>
</div>
