# Awesome-Webassembly-Runtimes

## Top Workflow Orchestration Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Data Pipelines, Durable Execution, DAG Scheduling, ML Workflows & Business Process Orchestration*  

**Last updated: October 2026**



This repository tracks notable **SaaS/hosted platforms** and **open-source projects** for **Workflow Orchestration**. These systems define, schedule, retry, and observe multi-step jobs—ETL/ELT, ML training, microservice sagas, and long-running business processes.



**Examples** include Apache Airflow, Astronomer, Prefect, Dagster Cloud, AWS Step Functions, Temporal Cloud, Flyte, Kubeflow, Google Cloud Composer, Azure Data Factory, and **Dagster** (`dagster-io/dagster`)—an orchestration platform for data assets.



**Open-source emphasis**: Workflow orchestration is strongly open source. **Airflow**, **Dagster**, **Prefect**, **Temporal**, **Flyte**, and **Argo Workflows** power production data and application pipelines worldwide. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Astronomer, Google Cloud Composer, Amazon MWAA](https://www.astronomer.io/)**  

  Managed Apache Airflow offerings—hosted control planes, scaling, and cloud integrations for data teams.



- **[Prefect Cloud, Dagster+](https://www.prefect.io/)**  

  Managed platforms around modern Python-native orchestrators with hybrid execution and observability.



- **[Temporal Cloud, AWS Step Functions, Azure Data Factory](https://temporal.io/)**  

  Durable execution and cloud-native workflow services for application and integration orchestration.



- **[Flyte (Union.ai), Kubeflow-oriented managed offerings](https://flyte.org/)**  

  Hosted ML and data workflow platforms built on open orchestrators.



- **[Other managed workflow platforms](https://aws.amazon.com/step-functions/)**  

  Additional serverless and enterprise orchestration services.



## Open-Source GitHub Projects



- **[Apache Airflow](https://github.com/apache/airflow)**  

  Leading open-source platform to programmatically author, schedule, and monitor workflows as DAGs—industry standard for data engineering.



- **[Dagster](https://github.com/dagster-io/dagster)**  

  Open orchestration platform centered on data assets—software-defined assets, strong typing, and development-oriented tooling.



- **[Prefect](https://github.com/PrefectHQ/prefect)**  

  Open Python-native workflow orchestration—dynamic flows, hybrid execution, and a modern developer experience.



- **[Temporal](https://github.com/temporalio/temporal)**  

  Open durable execution engine—workflows as code with automatic retries, timers, and versioning for reliable distributed processes.



- **[Flyte](https://github.com/flyteorg/flyte)**  

  Open Kubernetes-native workflow orchestrator optimized for data and ML pipelines with strong reproducibility.



- **[Argo Workflows](https://github.com/argoproj/argo-workflows)**  

  Open container-native workflow engine for Kubernetes—DAGs and steps as CRDs.



- **[Kubeflow Pipelines](https://github.com/kubeflow/pipelines)**  

  Open ML workflow platform on Kubernetes—pipeline authoring, experiment tracking, and recurring runs.



- **[Luigi](https://github.com/spotify/luigi)**  

  Open Python pipeline framework from Spotify—dependency-aware batch workflows, still widely used.



- **[Tekton](https://github.com/tektoncd/pipeline)**  

  Open Kubernetes-native CI/CD and pipeline primitives often reused for general workflow steps.



- **[Cadence](https://github.com/cadence-workflow/cadence)**  

  Open workflow orchestration engine (Uber origin) related in design lineage to Temporal.



- **[Mage / Kestra / Windmill](https://github.com/mage-ai/mage-ai)**  

  Emerging open orchestrators focused on developer UX, hybrid pipelines, and automation.



### Additional Strong Open-Source Options



- **Data engineering DAGs**: Apache Airflow or Dagster.

- **Python-first dynamic flows**: Prefect.

- **Durable application workflows**: Temporal.

- **K8s-native / ML**: Flyte, Argo Workflows, Kubeflow Pipelines.

- **Composable stacks**: Orchestrator → object storage → warehouse/lake → observability (OpenTelemetry).

- Managed clouds reduce ops for the control plane; execution often still runs in your VPC with open workers.



**Frameworks for building custom systems**:  

**Airflow** or **Dagster** for data asset pipelines; **Prefect** for flexible Python flows; **Temporal** for long-running business logic; **Flyte** / **Argo** on Kubernetes for ML and container steps.  

Fully open workflow orchestration is production-standard across startups and large enterprises.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS/hosted or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Workflow engines often hold credentials and can mutate production data. Apply least-privilege connections, secret management, and audit logging. Design tasks to be idempotent—retries will happen.

- Open-source orchestrators offer control and portability but require you to operate databases, queues, and workers. Managed platforms shift control-plane operations to the vendor. Neither replaces careful data contracts and failure handling.



---



**Made for data engineers, platform teams, and builders of reliable multi-step systems.**  

Let's expand open workflow orchestration while recognizing the managed convenience that hosted Airflow, Prefect, Dagster, and Temporal clouds deliver.
# Awesome-Webassembly-Runtimes

# Top WebAssembly Runtimes Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Wasm Execution Engines, Edge Compute, Component Model, WASI & Portable Server-Side WebAssembly*  
**Last updated: October 2026**

This repository tracks notable **SaaS/hosted platforms** and **open-source projects** for **WebAssembly Runtimes**. These systems execute Wasm modules outside the browser—on servers, at the edge, in plugins, and inside containers—with strong isolation and near-native speed.

**Examples** include Wasmer Cloud, Fermyon Cloud, Fastly Compute (Wasm), Cloudflare Workers, Cosmonic, Suborbital, Second State, Docker Wasm, Red Hat Wasm, Azure Wasm Labs, and **Wasmtime** (`bytecodealliance/wasmtime`)—a standalone JIT-style runtime for WebAssembly.

**Open-source emphasis**: Wasm runtimes are led by open source. **Wasmtime**, **Wasmer**, **WasmEdge**, **WAMR**, and **wasm3** form the core execution layer. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Cloudflare Workers, Fastly Compute](https://workers.cloudflare.com/)**  
  Edge compute platforms with first-class WebAssembly support for ultra-low-latency serverless workloads worldwide.

- **[Fermyon Cloud, Wasmer Cloud](https://www.fermyon.com/)**  
  Hosted platforms purpose-built for deploying and scaling Wasm applications and Spin-style microservices.

- **[Cosmonic, Second State, Suborbital-oriented services](https://cosmonic.com/)**  
  Wasm-centric application platforms and plugin runtimes for distributed and embeddable compute.

- **[Docker Wasm / cloud provider Wasm previews](https://docs.docker.com/)**  
  Container and cloud integrations that run Wasm modules alongside or instead of traditional containers.

- **[Other managed Wasm platforms](https://www.fastly.com/products/edge-compute)**  
  Additional edge and serverless offerings exposing Wasm as the unit of deployment.

## Open-Source GitHub Projects

### Core Runtimes

- **[Wasmtime](https://github.com/bytecodealliance/wasmtime)**  
  Standalone open JIT-style WebAssembly runtime from the Bytecode Alliance—WASI, Component Model, and production-focused embedding APIs.

- **[Wasmer](https://github.com/wasmerio/wasmer)**  
  Popular open Wasm runtime—multiple compiler backends, WASIX, and a strong focus on universal executables and packaging.

- **[WasmEdge](https://github.com/WasmEdge/WasmEdge)**  
  Cloud-native open Wasm runtime optimized for edge and service-mesh sidecars—CNCF project with rich extensions.

- **[WAMR (WebAssembly Micro Runtime)](https://github.com/bytecodealliance/wasm-micro-runtime)**  
  Lightweight open runtime from the Bytecode Alliance—suited to embedded devices and constrained environments.

- **[wasm3](https://github.com/wasm3/wasm3)**  
  Fast open WebAssembly interpreter—extremely portable and useful where JIT is unavailable.

- **[WasmKit / other experimental engines](https://github.com/search?q=webassembly+runtime)**  
  Community and research runtimes exploring alternate designs and languages.

### Platform Tooling & Standards

- **[Spin (Fermyon)](https://github.com/fermyon/spin)**  
  Open framework for building and running Wasm microservices with a developer-friendly DX.

- **[WASI / wasi-sdk](https://github.com/WebAssembly/wasi)**  
  Open system-interface standards and toolchains that let Wasm modules talk to files, clocks, and sockets portably.

- **[Component Model & wit-bindgen](https://github.com/bytecodealliance/wit-bindgen)**  
  Open tooling for the Wasm Component Model—language bindings and interface types for composable modules.

- **[wasm-tools](https://github.com/bytecodealliance/wasm-tools)**  
  Open CLI and libraries for inspecting, validating, and transforming Wasm binaries.

- **[wasm-pack / wasm-bindgen](https://github.com/rustwasm/wasm-pack)**  
  Open Rust-to-Wasm tooling widely used for both browser and server-side modules.

- **[Docker + Wasm runtimes integration](https://github.com/containerd/runwasi)**  
  Open containerd shims (e.g. runwasi) enabling Wasm workloads under container workflows.

- **[Extism](https://github.com/extism/extism)**  
  Open universal plugin system powered by WebAssembly—embed Wasm plugins in many host languages.

### Additional Strong Open-Source Options

- **General server/embed**: Wasmtime or Wasmer.
- **Edge / cloud-native**: WasmEdge.
- **Tiny / embedded**: WAMR or wasm3.
- **App framework**: Spin for microservice-style Wasm apps.
- **Plugins**: Extism for host-application extensibility.
- **Composable stacks**: Rust/Go/C → Wasm module → Wasmtime/Wasmer/WasmEdge → WASI or Component Model.
- Hosted edge platforms still lead for global PoP distribution and zero-ops scaling.

**Frameworks for building custom systems**:  
**Wasmtime** for standards-aligned embedding; **Wasmer** for packaging and WASIX; **WasmEdge** for cloud-native edge; **Spin** for app-level DX.  
Target **WASI** and the **Component Model** for portability.  
Fully open Wasm runtime stacks are production-ready for plugins, edge functions, and portable services.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS/hosted or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Wasm isolation is strong but not a substitute for defense in depth. Limit host capabilities granted via WASI, validate modules, and keep runtimes updated. Untrusted Wasm still requires careful capability design.
- Open-source runtimes offer transparency and embeddability. Managed edge platforms shift global distribution and scaling to the vendor. Neither replaces secure supply-chain practices for the modules you run.

---

**Made for systems engineers, edge developers, and teams building portable, isolated compute.**  
Let's expand open WebAssembly runtimes while recognizing the global edge footprint that commercial Wasm platforms deliver.
