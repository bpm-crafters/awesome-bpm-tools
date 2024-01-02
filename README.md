<div align="center">
<h1>Awesome BPM Tools</h1>

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Contribute](https://img.shields.io/badge/contribute-project-blue.svg)](https://github.com/camunda-community-hub/awesome-bpm-tools/pulls)

<hr />
<a href="CODE_OF_CONDUCT.md">Code of Conduct</a>&nbsp;&nbsp;&nbsp;
<a href="CONTRIBUTING.md">Contributing</a>
<hr />
</div>

A curated list of awesome BPM related projects. Inspired
by [awesome-camunda-8](https://github.com/camunda-community-hub/awesome-camunda-platform-8/blob/master/README.md).

Help us collect all things awesome about Business Process Management.

## Contents

- [Contents](#contents)
- [Books](#books-about-bpm)
- [BPMN Modeling Tools](#bpmn-modeling-tools)
- [Workflow Engines](#workflow-engines)
- [Dev Clients](#dev-clients)
- [Best Practices](#best-practices)
- [Testing](#testing)
- [Others](#others)
- [Contributing](#contributing)
- [License](#license)

# Awesome Projects

## Books about BPM

This section features some great books in the subject of business process management. With this list you can boost your
BPM game or start learning how you properly apply this methodology.

- [BPMN Method and Style](https://methodandstyle.com/bpmn-method-and-style/) by Bruce Silver:
  BPMN 2.0 is the industry standard diagramming language for business process models. The meaning of the business
  process diagram is the same, regardless of the tool used to create it. But creating models that are correct, complete,
  and clear demands more than a dictionary of BPMN shapes and symbols. It also requires a methodology for translating
  process logic consistently into the diagram. And it requires a measure of modeling style as well, conventions that
  ensure that the process logic is unambiguous from the diagram by itself. In short, “good BPMN” requires a disciplined
  approach called “method and style.”
- [Practical Process Automation](https://processautomationbook.com/) by Bernd Ruecker: In today’s IT architectures,
  microservices and serverless functions play an increasingly important role. But how can you create meaningful,
  comprehensive, and connected business solutions if the individual components are decoupled and independent by design?
  This book provides a framework through examples and practical advice, and reveals how you can design complex processes
  in such an environment to deliver true business value.
- [Process Driven Applications with BPMN](https://link.springer.com/book/10.1007/978-3-319-07218-0) by Volker Stiehl:
  How can we optimize differentiating business processes and exploit their full potential? Here Volker Stiehl provides
  answers, utilizing the various options that the BPMN (Business Process Model and Notation) standard offers for
  planning, implementing and monitoring processes.
  The book presents an approach for implementing an architecture for applications that strives to find a balance between
  development and maintenance costs, sustainability, scalability and fault tolerance; that meets flexibility
  requirements without becoming inordinately complex itself; and that keeps the end application as abstract as possible
  from the system landscape in which it operates.

## BPMN Modeling Tools and Frameworks

- [Introducing the Model Interchange Working Grouo](https://www.omgwiki.org/bpmn-miwg/doku.php): The Model Interchange
  Working Group (MIWG) is a group of vendors, consultants, and end-users who are interested in the exchange of models
  between tools in the BPMN 2.0 format. The group is open to all interested parties and is currently working on a set of
  test cases to validate the interchange of BPMN 2.0 models between tools. Besides, they are defining a set of
  guidelines for tool vendors to follow to ensure that their tools can interoperate with other tools.
- [bpmn-io](https://bpmn.io/): bpmn.io is a BPMN 2.0 rendering toolkit and web modeler. It helps you create BPMN
  diagrams in your browser.
- [Camunda Desktop Modeler](): The Camunda Desktop Modeler is a desktop application for modeling BPMN workflows and DMN
  decisions. It is based on the bpmn.io toolkit and is available for Windows, Mac and Linux.
- [5Minds Studio](https://processcube.io/docs/studio/installation): The 5Minds Studio is a desktop application for modeling BPMN workflows. It is written using
  Elektron and based on the bpmn.io toolkit.

## Workflow Engines

- [Zeebe](https://zeebe.io/): Zeebe is cloud-native developer-friendly workflow engine which relies on BPMN. At its core
  is open source, though it features several tools which are available in a paid version of the tool. Zeebe is
  horizontally
  scalable and fault-tolerant. Besides the capability to run BPMN it features a Decision Engine which is able to execute
  the DMN standard.
- [Camunda Platform 7](https://camunda.com/): Camunda Platform 7 is the predecessor of Zeebe. It is a reliable
  developer-friendly
- open source platform for workflow and decision automation that brings business users and software developers together.
  Camunda is based on Activiti and written in Java, hence it is a perfect match for Java EE and Spring
  while providing a powerful REST API and script language support. It can be embedded in any Java application or
  run as a service in the cloud or on an application server.
- [Kogito](https://kogito.kie.org/): Kogito is a cloud-native business automation technology for building cloud-ready
  business applications. Based on battle-tested runtime components (like Drools, jBPM, OptaPlanner), Kogito provides
  highly performant execution engine for cloud environments and brings domain-specific APIs to define your business
  logic.
- [Process Cube](https://processcube.io): The ProcessCube is an automation platform based on the BPMN Standard and
  written in NodeJS and Elektron that enables you to quickly develop high-quality solutions. Requirements can be
  documented, processes modeled and software developed in a single step. In addition, authorizations can be set. It is
  not open source but available for free. Besides it features various extension-points.

## Dev Clients

## Best Practices

- [BPM Manifesto](): The BPM Manifesto is a collection of 5 principles for applying BPM. It is being maintained by this
  community.

### BPMN Modelling Best-Practices

- [Creating readable process models](
  https://docs.camunda.io/docs/components/best-practices/modeling/creating-readable-process-models/)
- [Naming BPMN elements](https://docs.camunda.io/docs/components/best-practices/modeling/naming-bpmn-elements/)
- [Modelling beyond the happy path](https://docs.camunda.io/docs/components/best-practices/modeling/modeling-beyond-the-happy-path/)
- [Modelling with Situation Patterns](https://docs.camunda.io/docs/components/best-practices/modeling/modeling-with-situation-patterns/)
- [Building flexibility into BPMN models](https://docs.camunda.io/docs/components/best-practices/modeling/building-flexibility-into-bpmn-models/)

### Developer Best-Practices

## Testing

## Others

