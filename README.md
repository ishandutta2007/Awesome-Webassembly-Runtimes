# ⚡ Awesome WebAssembly Runtimes

<p align="center">
  <img src="assets/banner.svg" alt="Awesome WebAssembly Runtimes Banner" width="100%"/>
</p>

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a><a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Webassembly-Runtimes/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Webassembly-Runtimes?style=flat-square&color=gold" alt="GitHub_Stars"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Webassembly-Runtimes/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Webassembly-Runtimes?style=flat-square&color=blue" alt="GitHub Forks"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Webassembly-Runtimes/pulls"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Webassembly-Runtimes/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square" alt="License"/></a>
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

---

## 📖 Overview

A definitive, community-curated list of **WebAssembly (Wasm) Runtimes**, **Serverless Edge Platforms**, **Execution Engines**, and **WASI Tooling**. 

WebAssembly is moving far beyond web browsers. Server-side and edge Wasm provides near-instant cold starts (measured in microseconds), hardware-level capability sandboxing, tiny memory footprints, and language-agnostic portability across Linux, macOS, Windows, and embedded microcontrollers.

Whether you are evaluating stand-alone JIT engines (`Wasmtime`, `Wasmer`), cloud-native service meshes (`WasmEdge`), ultra-compact embedded interpreters (`wasm3`, `WAMR`), or global edge compute clouds (`Cloudflare Workers`, `Fastly Compute`), this guide provides technical comparisons, commercial pricing, free-tier limits, and real-time popularity metrics.

---

## 📑 Table of Contents

- [🌐 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [☁️ SaaS & Hosted Wasm Platforms](#️-saas--hosted-wasm-platforms)
- [🛠️ Open-Source GitHub Projects](#️-open-source-github-projects)
- [🧭 Architectural Decision Matrix](#-architectural-decision-matrix)
- [🤝 How to Contribute](#-how-to-contribute)
- [📈 Star History](#--star-history)
- [💖 Support & Contributing](#-support--contributing)
- [📜 Disclaimer](#-disclaimer)

---

## 🌐 Sector Overview & Market Dynamics

> **Market Size & Growth**: The global WebAssembly & serverless edge compute market was valued at **$5.2 Billion in 2024** and is projected to expand to **$26.8 Billion by 2032**, demonstrating a robust compound annual growth rate (**CAGR of ~22.8%**). Demand is driven by microservice cold-start reduction, secure multi-tenant plugin sandboxing, and ultra-low-latency edge AI inference.

> **Market Concentration**: The sector is currently **moderately fragmented**. High-bandwidth edge content delivery and global request routing are led by established edge CDN providers (Cloudflare, Fastly), while the server-side runtime, WASI standardization, container shims, and distributed component orchestration layers remain highly dynamic, contested, and innovated by dedicated open-source startups (Fermyon, Wasmer, Cosmonic) working alongside the Bytecode Alliance and CNCF.

---

## ☁️ SaaS & Hosted Wasm Platforms

The following hosted platforms and managed cloud runtimes offer turnkey WebAssembly execution outside the browser. Entries are sorted descending by company size (valuation or market capitalization).

| 🏢 Platform / Service | 💼 Company & Valuation / Revenue | ⚡ Key Capabilities & Execution Model | 💳 Starting Tier Pricing | 🎁 Free Tier / Free Trial Limits |
| :--- | :--- | :--- | :--- | :--- |
| **[Cloudflare Workers](https://workers.cloudflare.com/)** | Cloudflare, Inc. (NYSE: NET)<br>• **$35.2B Market Cap**<br>• $1.3B+ Annual Revenue | V8-based isolates with first-class Wasm compilation, global edge network across 330+ cities, KV storage, and sub-millisecond cold starts. | **$5.00 / month**<br>(Workers Paid includes 10M requests/mo + $0.30 per additional million requests) | **Free forever**:<br>• 100,000 requests / day<br>• 10ms CPU time / request<br>• Up to 100 worker scripts |
| **[Docker Wasm](https://docs.docker.com/desktop/wasm/)** | Docker, Inc.<br>• **$2.1B Valuation**<br>• $150M+ ARR | Container ecosystem integration running Wasm/WASI workloads alongside standard OCI containers via containerd and `runwasi`. | **$5.00 / user / month**<br>(Docker Pro billed annually at $60/yr or $7/mo monthly; includes advanced developer tooling) | **Free forever** (Docker Personal):<br>• Unlimited local Wasm engine execution<br>• 200 container pulls / 6 hours<br>• 1 private repository |
| **[Fastly Compute](https://www.fastly.com/products/edge-compute)** | Fastly, Inc. (NYSE: FSLY)<br>• **$1.12B Market Cap**<br>• $506M Annual Revenue | Standalone compiled WebAssembly execution based on Lucet/Wasmtime, delivering instant 35-microsecond cold starts at 100+ POPs. | **$50.00 / month**<br>(Or pay-as-you-go starting at $0.0000005/request + $0.00002/CPU-sec) | **Free recurring credit**:<br>• $50 / month recurring usage credit (equivalent to ~100M requests or ~2.5M CPU-sec) |
| **[Fermyon Cloud](https://www.fermyon.com/cloud)** | Fermyon Technologies, Inc.<br>• **$30M Valuation**<br>• $20M Series A raised | Purpose-built hosted serverless platform for Spin Wasm applications, key-value storage, SQLite integration, and edge AI inferencing. | **$10.00 / month**<br>(Developer Tier includes 50 apps, 15M requests/mo, custom domains, and managed DB) | **Free forever**:<br>• 5 active applications<br>• 100,000 requests / month<br>• 1 GB outbound bandwidth |
| **[Wasmer Cloud](https://wasmer.io/products/edge)** | Wasmer Inc.<br>• **$15M Valuation**<br>• $4.2M Seed raised | Universal cloud deployment running Wasm packages, WASIX extended POSIX syscalls, edge databases, and automatic global TLS domains. | **$12.00 / month**<br>(Wasmer Pro includes 10M requests/mo, 50GB data transfer, and custom domains) | **Free forever**:<br>• 3 published apps<br>• 1,000,000 requests / month<br>• 10 GB bandwidth & shared CPU |
| **[Cosmonic](https://cosmonic.com/)** | Cosmonic Corp.<br>• **$12M Valuation**<br>• $8.5M Seed raised | Managed distributed application platform based on CNCF wasmCloud; connects actor components across edge, hybrid, and multi-cloud nodes. | **$20.00 / month**<br>(Pro Developer Plan includes multi-cloud constellations, custom domains, and auto-scaling) | **30-day free trial**:<br>• 2 connected infrastructure hosts<br>• 25 actor/component instances<br>• 250 MB data transfer limit |
| **[Second State Flows.network](https://flows.network/)** | Second State Inc.<br>• **$8M Valuation**<br>• $4M Seed raised | Serverless WasmEdge execution platform automating AI agent workflows, GitHub automation, and event-driven LLM pipelines. | **$9.00 / user / month**<br>(Developer Tier includes 100 active flows, unlimited triggers, and priority execution) | **Free forever**:<br>• 5 active automation flows<br>• Up to 1,000 monthly event executions<br>• Standard community webhooks |

---

## 🛠️ Open-Source GitHub Projects

Curated open-source WebAssembly execution engines, runtimes, intermediate compilers, and standardization toolchains. **Sorted descending by real-time GitHub Stars_Count**.

1. **[Wasmer](https://github.com/wasmerio/wasmer)** [![GitHub_Stars](https://img.shields.io/github/stars/wasmerio/wasmer?style=social&color=white)](https://github.com/wasmerio/wasmer/stargazers)  
   🚀 Ultra-fast and lightweight WebAssembly runtime supporting multiple compiler backends (Cranelift, LLVM, Singlepass), WASIX extensions for full POSIX compatibility, and universal binary compilation.

2. **[Wasmtime](https://github.com/bytecodealliance/wasmtime)** [![GitHub_Stars](https://img.shields.io/github/stars/bytecodealliance/wasmtime?style=social&color=white)](https://github.com/bytecodealliance/wasmtime/stargazers)  
   ⚡ The standalone JIT WebAssembly runtime from the Bytecode Alliance. Industry benchmark for WASI implementation, high-security capability sandboxing, and official Wasm Component Model support.

3. **[AssemblyScript](https://github.com/AssemblyScript/assemblyscript)** [![GitHub_Stars](https://img.shields.io/github/stars/AssemblyScript/assemblyscript?style=social&color=white)](https://github.com/AssemblyScript/assemblyscript/stargazers)  
   🟦 TypeScript-like programming language designed specifically for compiling strictly-typed code directly into lightweight WebAssembly binaries.

4. **[TinyGo](https://github.com/tinygo-org/tinygo)** [![GitHub_Stars](https://img.shields.io/github/stars/tinygo-org/tinygo?style=social&color=white)](https://github.com/tinygo-org/tinygo/stargazers)  
   🐹 Go compiler optimized for constrained environments, microcontrollers, and ultra-compact WebAssembly / WASI builds with minimal runtime overhead.

5. **[WasmEdge](https://github.com/WasmEdge/WasmEdge)** [![GitHub_Stars](https://img.shields.io/github/stars/WasmEdge/WasmEdge?style=social&color=white)](https://github.com/WasmEdge/WasmEdge/stargazers)  
   🌐 CNCF-hosted, lightweight, high-performance WebAssembly runtime optimized for cloud-native edge computing, Kubernetes sidecars, and hardware-accelerated AI/LLM inference.

6. **[wasm-bindgen](https://github.com/rustwasm/wasm-bindgen)** [![GitHub_Stars](https://img.shields.io/github/stars/rustwasm/wasm-bindgen?style=social&color=white)](https://github.com/rustwasm/wasm-bindgen/stargazers)  
   🦀 Facilitates seamless, zero-copy high-level interactions between Rust data structures and WebAssembly host environments.

7. **[Binaryen](https://github.com/WebAssembly/binaryen)** [![GitHub_Stars](https://img.shields.io/github/stars/WebAssembly/binaryen?style=social&color=white)](https://github.com/WebAssembly/binaryen/stargazers)  
   ⚙️ WebAssembly compiler and toolchain infrastructure library providing comprehensive dead-code elimination, performance optimization, and IR generation passes.

8. **[WABT (WebAssembly Binary Toolkit)](https://github.com/WebAssembly/wabt)** [![GitHub_Stars](https://img.shields.io/github/stars/WebAssembly/wabt?style=social&color=white)](https://github.com/WebAssembly/wabt/stargazers)  
   🧰 The canonical tool suite for manipulating Wasm files, including `wasm2wat`, `wat2wasm`, `wasm-interp`, `wasm-objdump`, and `wasm-decompile`.

9. **[wasm3](https://github.com/wasm3/wasm3)** [![GitHub_Stars](https://img.shields.io/github/stars/wasm3/wasm3?style=social&color=white)](https://github.com/wasm3/wasm3/stargazers)  
   🚀 The fastest WebAssembly interpreter in existence. Fully portable C99 engine with zero JIT compilation lag, running on Arduino, ESP32, Raspberry Pi, iOS, and embedded chips.

10. **[Spin](https://github.com/spinframework/spin)** [![GitHub_Stars](https://img.shields.io/github/stars/spinframework/spin?style=social&color=white)](https://github.com/spinframework/spin/stargazers)  
    🌀 Open-source developer framework and CLI by Fermyon for building, testing, and deploying microservices and event-driven functions using WebAssembly components.

11. **[wazero](https://github.com/tetratelabs/wazero)** [![GitHub_Stars](https://img.shields.io/github/stars/tetratelabs/wazero?style=social&color=white)](https://github.com/tetratelabs/wazero/stargazers)  
    🟢 Pure Go WebAssembly runtime with zero CGO dependencies and full WASI support, making Go application embedding effortless and totally portable.

12. **[WAMR (WebAssembly Micro Runtime)](https://github.com/bytecodealliance/wasm-micro-runtime)** [![GitHub_Stars](https://img.shields.io/github/stars/bytecodealliance/wasm-micro-runtime?style=social&color=white)](https://github.com/bytecodealliance/wasm-micro-runtime/stargazers)  
    🔬 Ultra-small-footprint runtime from the Bytecode Alliance configurable as an interpreter, JIT, or AOT compiler for resource-constrained IoT devices.

13. **[Extism](https://github.com/extism/extism)** [![GitHub_Stars](https://img.shields.io/github/stars/extism/extism?style=social&color=white)](https://github.com/extism/extism/stargazers)  
    🔌 Universal WebAssembly plugin framework providing unified Host SDKs across 16+ programming languages to securely execute untrusted guest plugins.

14. **[Lunatic](https://github.com/lunatic-solutions/lunatic)** [![GitHub_Stars](https://img.shields.io/github/stars/lunatic-solutions/lunatic?style=social&color=white)](https://github.com/lunatic-solutions/lunatic/stargazers)  
    🌕 Erlang-inspired, actor-based runtime for WebAssembly combining preemptive scheduling, lightweight isolated processes, and fault-tolerant supervision trees.

15. **[wasmCloud](https://github.com/wasmCloud/wasmCloud)** [![GitHub_Stars](https://img.shields.io/github/stars/wasmCloud/wasmCloud?style=social&color=white)](https://github.com/wasmCloud/wasmCloud/stargazers)  
    ☁️ CNCF application runtime that lets developers compose portable WebAssembly actor components with decoupled capability providers across any infrastructure.

16. **[wasm-tools](https://github.com/bytecodealliance/wasm-tools)** [![GitHub_Stars](https://img.shields.io/github/stars/bytecodealliance/wasm-tools?style=social&color=white)](https://github.com/bytecodealliance/wasm-tools/stargazers)  
    🔧 Low-level CLI utilities and Rust libraries for inspecting, validating, mutating, stripping, and composing WebAssembly binaries and components.

17. **[wit-bindgen](https://github.com/bytecodealliance/wit-bindgen)** [![GitHub_Stars](https://img.shields.io/github/stars/bytecodealliance/wit-bindgen?style=social&color=white)](https://github.com/bytecodealliance/wit-bindgen/stargazers)  
    🧩 Multi-language binding generator for WebAssembly Interface Types (WIT), powering seamless inter-module communication in the Wasm Component Model.

18. **[runwasi](https://github.com/containerd/runwasi)** [![GitHub_Stars](https://img.shields.io/github/stars/containerd/runwasi?style=social&color=white)](https://github.com/containerd/runwasi/stargazers)  
    🐳 Containerd runtime shim enabling Kubernetes, Nomad, and Docker clusters to execute WebAssembly workloads directly as native Pods and containers.

19. **[Chicory](https://github.com/dylibso/chicory)** [![GitHub_Stars](https://img.shields.io/github/stars/dylibso/chicory?style=social&color=white)](https://github.com/dylibso/chicory/stargazers)  
    ☕ Native Java/JVM WebAssembly runtime with zero JNI bindings or native binary dependencies, bringing safe sandbox isolation into existing enterprise JVM applications.

---

## 🧭 Architectural Decision Matrix

| Requirement / Workload | Recommended Runtime | Rationale |
| :--- | :--- | :--- |
| **Production Server-Side Microservices** | **Wasmtime** or **Spin** | Strict WASI compliance, high JIT throughput with Cranelift, Component Model standards. |
| **Cross-Platform Universal Packaging** | **Wasmer** | Broadest OS support, WASIX for POSIX socket syscalls, integrated registry. |
| **Kubernetes & Cloud-Native Edge** | **WasmEdge** or **runwasi** | CNCF-aligned, containerd integration, hardware acceleration for LLMs (`wasi-nn`). |
| **Microcontrollers & Tiny IoT Devices** | **wasm3** or **WAMR** | Sub-megabyte binary footprint, interpreter mode with zero compilation overhead. |
| **Embed Sandboxed Plugins in Host Apps** | **Extism** | Prebuilt Host SDKs in Go, Rust, Python, Node.js, C#, PHP, Ruby, and Java. |
| **Pure Go Application Stacks** | **wazero** | Eliminates CGO dependency hurdles; pure Go compilation into a single static binary. |
| **Enterprise Java / JVM Integration** | **Chicory** | Pure JVM bytecode execution without native C++ libraries or OS architecture mismatch. |

---

## 🤝 How to Contribute

Contributions are warmly welcome! To add or update an entry:

1. 🍴 Fork this repository: [Awesome-Webassembly-Runtimes](https://github.com/ishandutta2007/Awesome-Webassembly-Runtimes)
2. 📝 Add or edit entries in `README.md` following the existing format.
3. 🔎 Provide official project links, concise technical descriptions, and factual pricing/limits.
4. 🚀 Open a Pull Request detailing the additions or updates.

Check out our curated meta-list at **[Awesome-Awesome-Awesome](https://github.com/ishandutta2007/Awesome-Awesome-Awesome)** for more top developer resources!

---

##  Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Webassembly-Runtimes&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Webassembly-Runtimes&type=date&legend=top-left)

---

## 💖 Support & Contributing

Thank you for visiting and supporting **Awesome WebAssembly Runtimes**! 🙏

If you found this repository helpful for your projects, research, or architecture decisions, please consider supporting us:
- ⭐ **Star** this repository to help other developers and platform engineers discover it
- 🍴 **Fork & Share** with your teammates, communities, and developer networks
- 📬 Join discussions and connect on [Discord](https://discord.gg/jc4xtF58Ve)
- ☕ **Sponsor & Buy a Coffee**: Support ongoing research, updates, and open-source maintenance directly on the [GitHub Sponsors Dashboard](https://github.com/sponsors/ishandutta2007)

---

## 📜 Disclaimer

- This is a **community-curated** educational directory — not an official endorsement of any vendor or tool.
- WebAssembly isolation provides strong memory safety, but defense in depth remains essential. Restrict host capabilities granted through WASI interfaces, validate untrusted binaries, and keep your host runtimes updated.
- All product names, logos, and trademarks belong to their respective copyright holders.

## Star History

<a href="https://star-history.com/#ishandutta2007/Awesome-Webassembly-Runtimes&Timeline" align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/ishandutta2007_Awesome-Webassembly-Runtimes_growth.svg">
    <img alt="Star History Chart" src="assets/ishandutta2007_Awesome-Webassembly-Runtimes_growth.svg">
  </picture>
</a>
