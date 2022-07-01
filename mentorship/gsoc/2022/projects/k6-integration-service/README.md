GSoC 2022 - K6 Integration Service
==========

K6 is an open-source tool widely used for load testing.
With Keptn’s Quality gates, we can automate the process of evaluating the results of the test and also monitor them.
Keptn already supports JMeter, Locust, Litmus Chaos, and others.
This project will enable users to use K6 for performance testing.
Further goals include adding SLI and SLO compliance using Prometheus which K6 supports natively.

## Project team

<!-- TODO: add GitHub and social media links here -->

- Contributor: Jainam Shah - [GitHub](https://github.com/jainammm/) | [LinkedIn](https://www.linkedin.com/in/jainammm/) | [Twitter](https://twitter.com/jvenommm)
- Mentors:
  - Pepe Cano - [GitHub](https://github.com/ppcano/) | [LinkedIn](https://www.linkedin.com/in/ppcano/) | [Twitter](https://twitter.com/ppcano_)
  - Adam Gardner - [GitHub](https://github.com/agardnerit/) | [LinkedIn](https://www.linkedin.com/in/agardner1/)

## Contacts

- Slack: `#wg-k6-integrations` on [Keptn Slack](https://keptn.sh/community/#slack)

## Details

Support for K6 will help extend Keptn community users to switch/use it as performance testing tool. 
K6 is considered to be a modern tool for DevOps like Keptn, so the community might be inclined towards using it. 

Some of the features of K6 include: 
* It has good resource utilization and one load generator can simulate tens of thousands of virtual users
* It is code-driven, with JavaScript as scripting language
* K6 has native support for Prometheus

Thresholds in K6 are used for some specific pass/fail criteria. This feature is very commonly used. Based on passed/failed of Thresholds results, we'll return the state to the Keptn control plane.

The K6 service will suscribe to the `sh.keptn.event.test.triggered` CloudEvent and execute the Load Testing. K6 will write the metrics to Prometheus for further step of SLO evaluation.

## Project Resources

* [Repository](https://github.com/keptn-sandbox/k6-service)
* [SCRUM Board](https://github.com/keptn-sandbox/k6-service/projects)
* Meeting Schedule
  * Every Thursday @ 8:30 UTC
  * [Zoom Link](https://dynatrace.zoom.us/j/96378132758?pwd=Z0NRbXhxNlJiSjRqMkd5cmlLWEJMUT09)
* [Meeting Minutes](https://docs.google.com/document/d/1A3gbtQ6-YOTpO3v_ltBgHWTODFt93zByHXWVJ6r0jcg/edit?usp=sharing)

## References

* [Project page at GSoC website](https://summerofcode.withgoogle.com/programs/2022/projects/0xICJhw8)
