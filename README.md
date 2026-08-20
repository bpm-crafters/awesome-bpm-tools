# Awesome BPM Tools [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of great **BPM(N)** projects — process engines, supporting libraries, and modeling solutions. It focuses primarily on **process automation** and everything around it: running, building, testing and operating executable BPMN processes. Centered on the Camunda ecosystem as well as Operaton, CIB seven and the open-source tooling built around it. Automation frameworks listed here are Java-based.

## Contents

- [Process Engines](#process-engines)
- [Process Engine Clients & Frameworks](#process-engine-clients--frameworks)
- [Modelers](#modelers)
- [Modeling Toolkits & Linting](#modeling-toolkits--linting)
- [Testing & Coverage](#testing--coverage)
- [Code Generation & Developer Tooling](#code-generation--developer-tooling)
- [Task Management & UIs](#task-management--uis)
- [Integrations & Connectors](#integrations--connectors)
- [AI & Analytics](#ai--analytics)
- [Presentation Tooling](#presentation-tooling)
- [Code of Conduct](#code-of-conduct)

## Process Engines

*The runtimes that actually execute BPMN 2.0 (and DMN) processes — the heart of any BPM stack.*

- [Camunda 8 / Zeebe](https://github.com/camunda/camunda) - Cloud-native, horizontally scalable process orchestration engine.
- [Camunda 7](https://github.com/camunda/camunda-bpm-platform) - Established BPMN & DMN workflow engine (Community Edition); upstream is end-of-life, but lives on through the community forks below.
- [Operaton](https://github.com/operaton/operaton) - Community-owned, Apache-2.0 fork of Camunda 7 with Cockpit, Admin, Tasklist and REST API.
- [CIB seven](https://github.com/cibseven/cibseven) - Permanent Camunda 7 fork by CIB software with long-term support and an easy migration path.

See also: the [OMG BPMN Model Interchange Working Group (MIWG)](https://www.omgwiki.org/bpmn-miwg/doku.php) regularly tests vendor engines and tools against each other for real BPMN model interoperability — a useful, vendor-neutral check on standard compliance.

## Process Engine Clients & Frameworks

*Libraries your application code talks to when starting, completing and querying BPMN processes. These engine-agnostic frameworks — BPM Crafters (maintained by this list's own org, see [bpm-crafters.dev](https://bpm-crafters.dev)) and VanillaBP — let you write that logic once and run it on different engines, easing migrations and avoiding lock-in.*

- [process-engine-api](https://github.com/bpm-crafters/process-engine-api) - Unified, engine-neutral API for implementing process applications.
- [process-engine-adapters-camunda-7](https://github.com/bpm-crafters/process-engine-adapters-camunda-7) - Process Engine API adapter for Camunda 7 (embedded & remote).
- [process-engine-adapters-camunda-8](https://github.com/bpm-crafters/process-engine-adapters-camunda-8) - Process Engine API adapter for Camunda 8.
- [process-engine-adapters-cib-seven](https://github.com/bpm-crafters/process-engine-adapters-cib-seven) - Process Engine API adapter for CIB seven.
- [process-engine-worker](https://github.com/bpm-crafters/process-engine-worker) - Annotation-based service task worker with a Spring Boot starter.
- [VanillaBP](https://github.com/vanillabp) - Engine-agnostic framework to write BPMN process logic once and run it on different engines, with a Spring Boot integration and adapters for Camunda 7 & 8.

Note: every engine also ships its own official, engine-specific client (e.g. Camunda 7's Spring Boot Starter, Camunda 8's Spring SDK) — check the engine's own repo under **Process Engines** above for those.

## Modelers

*Ready-to-use applications you open and draw BPMN, DMN and Form diagrams in directly — no coding required.*

- [Miragon BPMN Modeler](https://github.com/Miragon/bpmn-modeler) - BPMN modeler right in your IDE — supports VS Code & IntelliJ, with support for Camunda 7, Camunda 8, Operaton and CIB seven.
- [Camunda Modeler](https://github.com/camunda/camunda-modeler) - Cross-platform desktop app for modeling BPMN, DMN and Forms.

## Modeling Toolkits & Linting

*The embeddable web toolkits behind most browser-based modelers, plus the linters that catch modeling mistakes before deployment — for developers building or validating their own tooling rather than end users drawing diagrams.*

- [bpmn-js](https://github.com/bpmn-io/bpmn-js) - BPMN 2.0 rendering toolkit and web modeler, embeddable in any web app.
- [dmn-js](https://github.com/bpmn-io/dmn-js) - DMN 1.3 viewer and editor for decision tables, literal expressions and DRDs.
- [form-js](https://github.com/bpmn-io/form-js) - JSON-based form viewer, editor and simulator for process user tasks.
- [diagram-js](https://github.com/bpmn-io/diagram-js) - Core library for displaying and modifying diagrams on the web; foundation of bpmn-js and dmn-js.
- [bpmn-js-properties-panel](https://github.com/bpmn-io/bpmn-js-properties-panel) - Properties panel to edit generic and Camunda-specific BPMN element properties in bpmn-js.
- [camunda-bpmn-js](https://github.com/camunda/camunda-bpmn-js) - Camunda-flavored bpmn-js distributions (Camunda 7 & 8) with properties panel and linting preconfigured.
- [bpmnlint](https://github.com/bpmn-io/bpmnlint) - Validate BPMN diagrams against configurable lint rules (CLI & library).
- [bpmnlint-rules](https://github.com/Miragon/bpmnlint-rules) - Collection of reusable bpmnlint rules for validating BPMN diagrams against common modeling conventions.

## Testing & Coverage

*Verify that your BPMN processes take the right paths before they reach production.*

- [zeebe-process-test](https://github.com/camunda/zeebe-process-test) - Official library for unit-testing BPMN processes on Camunda 8 (Zeebe).
- [Holunda · c7-jgiven](https://github.com/holunda-io/c7/tree/develop/c7-testing/c7-jgiven) - BDD-style stages and scenarios for testing Camunda 7 processes with the JGiven testing framework.

## Code Generation & Developer Tooling

*Keep BPMN models and the surrounding code in sync and automate the BPM developer workflow.*

- [bpmn-to-code](https://github.com/Miragon/bpmn-to-code) - Gradle/Maven plugin that generates typed Process APIs (Kotlin/Java) from BPMN models.
- [bpmn-to-image](https://github.com/bpmn-io/bpmn-to-image) - Convert BPMN and DMN diagrams to SVG, PNG or PDF from the command line.
- [camunda-modeler-i18n-plugin](https://github.com/Miragon/camunda-modeler-i18n-plugin) - Translates the Camunda Modeler UI into additional languages.
- [camunda-dmn-xlsx](https://github.com/camunda-community-hub/camunda-dmn-xlsx) - Convert XLSX spreadsheets to and from DMN decision tables.

## Task Management & UIs

*Surface the BPMN user tasks a process creates to the people who need to work on them.*

- [camunda-bpm-taskpool / Polyflow](https://github.com/holunda-io/camunda-bpm-taskpool) - Pools user tasks and process-related business objects for building task lists.
- [VanillaBP · business-cockpit](https://github.com/vanillabp/business-cockpit) - BPMS user interface for microservice environments.

## Integrations & Connectors

*Wire BPMN processes to the external systems, protocols and events they orchestrate (Java).*

- [Camunda Connectors](https://github.com/camunda/connectors) - Connector SDK and out-of-the-box connectors to integrate Camunda 8 with external systems.
- [camunda-platform-7-keycloak](https://github.com/camunda-community-hub/camunda-platform-7-keycloak) - Keycloak identity provider plugin for Camunda 7.
- [zeebe-kafka-exporter](https://github.com/camunda-community-hub/zeebe-kafka-exporter) - Export Zeebe events to Apache Kafka.

## AI & Analytics

*Understand, analyse and improve BPMN processes with AI- and MCP-based tooling.*

- [bpmn-iq](https://github.com/Miragon/bpmn-iq) - AI-first analytics for BPMN models, exposed via MCP for LLM-driven analysis.
- [miragon-ai](https://github.com/Miragon/miragon-ai) - Process analytics and operations for Camunda 7-based engines over the Model Context Protocol.
- [operaton-mcp](https://github.com/operaton/operaton-mcp) - MCP server for Operaton.

## Presentation Tooling

*Show live BPMN/DMN diagrams in talks and docs instead of blurry screenshots.*

- [slidev](https://github.com/slidevjs/slidev) - Markdown-based presentation slides framework for developers.
- [slidev-addon-bpmn](https://github.com/emaarco/slidev-addon-bpmn) - Display BPMN diagrams directly in Slidev, powered by bpmn.io.
- [slidev-addon-dmn](https://github.com/emaarco/slidev-addon-dmn) - Display DMN diagrams directly in Slidev, powered by dmn.io.

## Code of Conduct

This project adheres to a [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold it.

## Contributing

Contributions are welcome! Please read the [Contributing guidelines](CONTRIBUTING.md) before opening a pull request.
