<div align="center">

<img src="https://i.ibb.co/N6m72sYQ/AWLabs.png" alt="Adventure Wave Labs" width="600">

![Adventure Wave Labs](https://img.shields.io/badge/Adventure_Wave_Labs-Builder-ff6b6b?style=for-the-badge)
![Claude](https://img.shields.io/badge/-Claude-2b2b2b?style=flat-square&logo=anthropic&logoColor=d4a27f)
![Rust](https://img.shields.io/badge/-Rust-2b2b2b?style=flat-square&logo=rust&logoColor=dea584)
![License](https://img.shields.io/badge/license-MIT-orange?style=for-the-badge)

**We build open-source developer tooling for the Claude and agentic AI ecosystem.**

*Founded by the creator of [turbo-flow](https://github.com/marcuspat/turbo-flow) — the autonomous multi-agent dev environment used by engineers who ship like a team of one.*

[![Website](https://img.shields.io/badge/Website-adventurewavelabs.space-2b2b2b?style=flat-square)](https://adventurewavelabs.space)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-2b2b2b?style=flat-square&logo=linkedin&logoColor=0A66C2)](https://linkedin.com/in/marcuspatman)
[![YouTube](https://img.shields.io/badge/-YouTube-2b2b2b?style=flat-square&logo=youtube&logoColor=FF0000)](https://youtube.com/@marcuspatmanagentics)
[![X](https://img.shields.io/badge/-X-2b2b2b?style=flat-square&logo=x&logoColor=white)](https://x.com/marcuspat)

</div>

---

## What is Adventure Wave Labs?

Adventure Wave Labs (AWL) is the open-source lab behind [Turbo-Flow](https://github.com/marcuspat/turbo-flow) and its supporting toolchain — CLIs, agentic loop runners, and code-intelligence engines that let a single engineer operate a full agentic development workflow on top of Claude Code. Everything here is Rust-first, MCP-native, and built to run in real terminals against real codebases — not demos.

## What We Build

### Developer Tooling

| Repo | Lang | What it does |
|---|---|---|
| [cloop](https://github.com/adventurewave-labs/cloop) | Rust | Agentic loops for Claude Code — zero-dependency CLI that wraps `claude --print` in a configurable loop until tests pass, a marker appears, or N iterations |
| [secret-scan](https://github.com/adventurewave-labs/secret-scan) | Rust | Regex-based secret scanner for CI pipelines |
| [codescope](https://github.com/adventurewave-labs/codescope) | Rust | Single-binary code intelligence engine for AI coding agents — tree-sitter, MCP, CLI |
| [loopgen-rs](https://github.com/adventurewave-labs/loopgen-rs) | Rust | Agentic loop runner for Claude Code |
| [preflight-integration-tester](https://github.com/adventurewave-labs/preflight-integration-tester) | Python | Pre-deploy integration test harness |
| [turbo-flow-wizard](https://github.com/adventurewave-labs/turbo-flow-wizard) | Shell | Guided setup wizard for turbo-flow — interactive generator for project-specific CLAUDE.md configs |

#### In motion

| [<img src="https://raw.githubusercontent.com/adventurewave-labs/cloop/main/cloop-demo.gif" width="420" height="340" alt="cloop wizard creating a fix-tests loop, then listing and showing it">](https://github.com/adventurewave-labs/cloop) | [<img src="https://raw.githubusercontent.com/adventurewave-labs/codescope/main/demo.gif" width="420" height="340" alt="codescope indexing itself and answering blast-radius queries">](https://github.com/adventurewave-labs/codescope) |
|:---:|:---:|
| *cloop — agentic loops for Claude Code* | *codescope — code intelligence for agents* |
| [<img src="https://raw.githubusercontent.com/adventurewave-labs/secret-scan/main/docs/secretscan-demo.gif" width="420" height="340" alt="secretscan finding 6 planted secrets in a demo repo">](https://github.com/adventurewave-labs/secret-scan) | [<img src="https://raw.githubusercontent.com/adventurewave-labs/loopgen-rs/main/demo.gif" width="420" height="340" alt="loopgen rendering an agentic loop harness with --dry-run">](https://github.com/adventurewave-labs/loopgen-rs) |
| *secret-scan — CI secret scanner* | *loopgen-rs — agentic loop runner* |
| [<img src="https://raw.githubusercontent.com/adventurewave-labs/preflight-integration-tester/main/demo.gif" width="420" height="340" alt="preflight-integration-tester running a real readiness diagnostic — 97% GO, 3 middleware gaps found">](https://github.com/adventurewave-labs/preflight-integration-tester) | |
| *preflight-integration-tester — AI readiness diagnostic* | |

### Lab / Demos

Experiments, proofs of concept, and agentic demos. Production-grade code, not production-grade scope.

| Repo | What it explores |
|---|---|
| [agentic-powered-golden-path-demo](https://github.com/adventurewave-labs/agentic-powered-golden-path-demo) | NL → GitOps deployment via golden-path workflows (ArgoCD + OpenRouter) |
| [AI-Kubernetes-API-Generator-Demo](https://github.com/adventurewave-labs/AI-Kubernetes-API-Generator-Demo) | NL → Kubernetes API generation |

---

## FAQ

**What is Adventure Wave Labs?**
An open-source lab building developer tooling for the Claude and agentic AI ecosystem — CLIs, agentic loop runners, and code-intelligence tools used alongside Claude Code.

**What is Turbo-Flow?**
Turbo-Flow is AWL founder Marcus Patman's agentic development environment — 215+ MCP tools, cross-session memory, and per-agent git-worktree isolation, bootstrapped with one command on DevPod, Codespaces, or Rackspace Spot. See [marcuspat/turbo-flow](https://github.com/marcuspat/turbo-flow).

**Is this tooling used in production?**
Yes — `secret-scan` and `preflight-integration-tester` run in real CI/CD and pre-deploy pipelines; the rest of the toolchain is dogfooded daily inside Turbo-Flow itself.

---

## Stack

Rust · Shell · Python · Claude Code · MCP · Kubernetes · Terraform

Founder-published crates on [crates.io](https://crates.io/users/marcuspat) — 11,000+ total downloads: [secretscan](https://crates.io/crates/secretscan) · [cargo-forge](https://crates.io/crates/cargo-forge) · [netrain](https://crates.io/crates/netrain) · [cargocrypt](https://crates.io/crates/cargocrypt) · [k8s-netinspect](https://crates.io/crates/k8s-netinspect) · [file-hasher](https://crates.io/crates/file-hasher)

---

<div align="center">

**Built & Presented by Adventure Wave Labs**

Built by [Marcus Patman](https://github.com/marcuspat) — Principal Agentic Engineer
LATAM AI solutions at [creandotumatrix-labs](https://github.com/creandotumatrix-labs)

📧 marcus@adventureonthewave.com · [adventurewavelabs.space](https://adventurewavelabs.space) · [LinkedIn](https://linkedin.com/in/marcuspatman) · [X @marcuspat](https://x.com/marcuspat) · [YouTube](https://youtube.com/@marcuspatmanagentics)

</div>
