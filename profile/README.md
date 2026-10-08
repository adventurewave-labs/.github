<div align="center">

<img src="https://raw.githubusercontent.com/adventurewave-labs/.github/main/profile/banner.svg" alt="Adventurewave Labs — animated banner" width="100%">

![Adventure Wave Labs](https://img.shields.io/badge/Adventure_Wave_Labs-Builder-ff6b6b?style=for-the-badge)
![Claude](https://img.shields.io/badge/-Claude-2b2b2b?style=flat-square&logo=anthropic&logoColor=d4a27f)
![Rust](https://img.shields.io/badge/-Rust-2b2b2b?style=flat-square&logo=rust&logoColor=dea584)
![License](https://img.shields.io/badge/license-MIT-orange?style=for-the-badge)

**We build open-source developer tooling for the Claude and agentic AI ecosystem.**

*Founded by [Marcus Patman](https://github.com/marcuspat) — creator of [Turbo Flow](https://github.com/marcuspat/turbo-flow) (versions 1–4 were a full multi-agent dev environment; v5 is the rules layer for AI-written code) and [Turbo Rig](https://turbo-rig.com), the lab's current agentic coding rig.*

[![Website](https://img.shields.io/badge/Website-adventurewavelabs.space-2b2b2b?style=flat-square)](https://adventurewavelabs.space)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-2b2b2b?style=flat-square&logo=linkedin&logoColor=0A66C2)](https://linkedin.com/in/marcuspatman)
[![YouTube](https://img.shields.io/badge/-YouTube-2b2b2b?style=flat-square&logo=youtube&logoColor=FF0000)](https://youtube.com/@marcuspatmanagentics)
[![X](https://img.shields.io/badge/-X-2b2b2b?style=flat-square&logo=x&logoColor=white)](https://x.com/marcuspat)

</div>

---

## What is Adventure Wave Labs?

Adventure Wave Labs (AWL) is the open-source lab behind [Turbo-Flow](https://github.com/marcuspat/turbo-flow) and its supporting toolchain — CLIs, agentic loop runners, and code-intelligence engines that let a single engineer operate a full agentic development workflow on top of Claude Code. Everything here is Rust-first, MCP-native, and built to run in real terminals against real codebases — not demos.

## The Turbo Rig Stack - A Complete Agentic System

The successor to Turbo Flow — not more agents, but the harness that governs them: **Triangle + Spine + Loop**. Swappable lanes (builder / reviewer / reserve) under one shared constitution, a review gate **cross-checked across model families** with fail-closed verdicts, worktree isolation for parallel writers, git-versioned cross-session memory — and the merge button always in human hands.

| Tool | Stars | Lang | Purpose |
|---|---|---|---|
| [**turbo-rig**](https://github.com/marcuspat/turbo-rig) | — | Shell / Python | The full rig: a ten-law constitution, `review.sh` — the review gate with token accounting, `wt.sh` worktrees, `secret.sh` keychain, git-versioned `memory/`, specs and runbooks. One command installs and wires it all. *Private repo — beta.* |
| [**Turbo Brain v2**](https://github.com/adventurewave-labs/turbo-brain-v2) | — | Python / Shell | The rig's memory plane — an owned context vault: plain markdown in git, served read-only over MCP so a session starts with the context it needs instead of asking for it. Capture is a pure text PUT; schema lint, secret scan, client deny-list and agent-poison tripwires gate what enters, and budget-capped distill waves land as PRs under a protected main. *Private repo — v1.2.0.* |
| [**turbo-rig.com**](https://turbo-rig.com) | — | — | The product page: the full methodology — why builder ≠ reviewer, the three execution planes (laptop / VPS / Codespaces), and the eight-station loop that ends in a human merge. |
| [**Deep-dive**](https://turbo-rig-deep-dive.vercel.app) | — | — | Technical walkthrough with 11 SVG diagrams — triangle, spine, planes, and loop, section by section. |
| [**Deep-dive 3D**](https://turbo-rig-deep-dive-3d.vercel.app) | — | — | The same architecture as an explorable 3D scene — the loop, the triangle, the gate, the data gravity well, the planes, and the automation ring. |
| [**7-Day Stats**](https://turbo-rig-stats-only-sept14-21.vercel.app) | — | — | One engine, Sept 14–21, 2026: 141 PRs merged across 5 repos, 868 gate verdicts (79% of them REVISE), 104 worktree lanes, 4.21B tokens, $416 total review spend. |
| [**Beta**](https://turbo-rig-beta.vercel.app) | — | — | Request access to the private repo during the beta. |

---

## The Turbo-Flow Stack - The Rules Layer for AI-Written Code (v5)

| Tool | Stars | Lang | Purpose |
|---|---|---|---|
| [turbo-flow](https://github.com/marcuspat/turbo-flow) | ![](https://img.shields.io/github/stars/marcuspat/turbo-flow?style=flat-square&label=%E2%AD%90) | Shell / Python | Versions 1–4 (2025–2026): full agentic dev environment — 215+ MCP tools (via [Ruflo v3.5](https://github.com/ruvnet/ruflo) by [ruvnet](https://github.com/ruvnet)), cross-session memory (Beads), codebase knowledge graph (GitNexus), per-agent git-worktree isolation, one-command bootstrap on DevPod, Codespaces, or Rackspace Spot. Since v5: rig-lite — a portable bash-only governance kit (fail-closed cross-model review gate, constitution, git-versioned memory) for any repo and any coding agent. Site: [turboflow.space](https://turboflow.space) · Academy: [Turbo Flow University](https://www.turboflowuniversity.space) |
| [turbo-flow-wizard](https://github.com/adventurewave-labs/turbo-flow-wizard) | ![](https://img.shields.io/github/stars/adventurewave-labs/turbo-flow-wizard?style=flat-square&label=%E2%AD%90) | Shell | Guided setup wizard for turbo-flow — interactive generator for project-specific CLAUDE.md configs. 12 app types, 7 methodologies, 19 feature sets. |
| [loopgen](https://github.com/adventurewave-labs/loopgen-rs) | ![](https://img.shields.io/github/stars/adventurewave-labs/loopgen-rs?style=flat-square&label=%E2%AD%90) | Rust | Agentic loops for Claude Code — wizard, TOML configs, bash export, LOOP_STATUS protocol. Published on [crates.io](https://crates.io/crates/loopgen). |
| [tf-verify.sh](https://github.com/marcuspat/turbo-flow/blob/main/devpods/tf-verify.sh) | — | Shell | 50+ quality gates across 12 verification phases — dependency integrity, deployment state, artifact validation, and environment checks. Bundled in turbo-flow `devpods/`. |
| [turbo-brain-v2](https://github.com/adventurewave-labs/turbo-brain-v2) | — | Python / Shell | The stack's knowledge vault — the same Turbo Brain v2 listed in the Turbo Rig Stack table above; one repo, serving Claude Code, Cowork and Turbo Flow over read-only MCP (`brain_search`, `brain_context`, `brain_verify`). *Private repo — v1.2.0.* |

### In motion

| [<img src="https://raw.githubusercontent.com/marcuspat/marcuspat/main/demos/turbo-flow-demo.gif" width="420" alt="turbo-flow running the real codespace_setup.sh chain, then a live tmux tour and claude launch">](https://github.com/marcuspat/turbo-flow) | [<img src="https://raw.githubusercontent.com/marcuspat/marcuspat/main/demos/turbo-flow-wizard-demo.gif" width="420" alt="turbo-flow-wizard generating a CLAUDE.pre from a live Q&A session">](https://github.com/adventurewave-labs/turbo-flow-wizard) |
|:---:|:---:|
| *turbo-flow — real install, real tmux workspace, real claude launch* | *turbo-flow-wizard — interactive CLAUDE.md generator* |

| [<img src="https://raw.githubusercontent.com/adventurewave-labs/loopgen-rs/main/demo.gif" width="650" alt="loopgen driving an agentic loop with --dry-run">](https://github.com/adventurewave-labs/loopgen-rs) |
|:---:|
| *loopgen — agentic loops for Claude Code: wizard, TOML, bash export* |

---

## What We Build

### DevOps / Infrastructure

Autonomous agents, reliability tooling, and infrastructure posture scanning. These projects sit between your CI/CD pipeline and your fleet — they watch, diagnose, heal routine failures, and gate deployments on cluster posture without human intervention.

<p align="center">
  <a href="https://github.com/adventurewave-labs/ansible-heal-agent">
    <img src="https://raw.githubusercontent.com/adventurewave-labs/ansible-heal-agent/main/docs/demo.svg" alt="ansible-heal-agent demo — heals a broken baseline in 7 seconds" width="640">
  </a>
</p>

<p align="center"><em>ansible-heal-agent heals 3 seeded failures (stale hostname, removed <code>apt_key</code>, undefined <code>nginx_port</code>) and lands 3 conventional commits in 7 seconds.</em></p>

| Repo | Lang | What it does |
|---|---|---|
| [ansible-heal-agent](https://github.com/adventurewave-labs/ansible-heal-agent) | Python | Autonomous agent that scans Ansible logs, diagnoses routine failures (stale hostname, removed module, undefined variable), patches the playbook / inventory / vars, commits via conventional commits, and re-runs the pipeline. LLM-first (GLM-4-Plus via `z-ai-web-dev-sdk`) with a deterministic rule-based fallback, YAML validation before write, and a full Markdown transcript for human audit. `make demo` heals a broken baseline end-to-end in about 7 seconds. |
| [noip-scanner](https://github.com/adventurewave-labs/noip-scanner) | TypeScript | NOIP — read-only Kubernetes posture scanner. 15 deterministic checks (pod security, NetworkPolicy, RBAC, CIS L1 workload subset) with NSA/CISA and NIST reference mappings; live cluster, offline manifest, or multi-context fleet scans; JSON / MD / SARIF / HTML reports in EN/ES; `--fail-on` pipeline gating; audit evidence bundles with DSSE signing; ValidatingAdmissionPolicy generation. Golden-tested against a real kind cluster in CI. |

#### In motion

<p align="center">
  <a href="https://github.com/adventurewave-labs/noip-scanner">
    <img src="https://raw.githubusercontent.com/adventurewave-labs/noip-scanner/main/docs/demo.gif" alt="noip scanning a seeded kind cluster — live scan (score 35/100, 17 findings), --fail-on pipeline gate, evidence bundle + verify-bundle, ValidatingAdmissionPolicy generation, Spanish report" width="640">
  </a>
</p>

<p align="center"><em>noip-scanner scanning a seeded kind cluster — live scan (score 35/100, 17 findings), <code>--fail-on</code> exiting <code>2</code> as a pipeline gate, evidence bundle + <code>verify-bundle</code>, ValidatingAdmissionPolicy generation, and a Spanish report.</em></p>

### Developer Tooling

CLIs and engines that plug into the agentic workflow — an agentic loop runner, a CI secret scanner, a code-intelligence engine, and a pre-deploy test harness. Each one shown doing real work against a real target in the grid below.

| Repo | Lang | What it does |
|---|---|---|
| [loopgen-rs](https://github.com/adventurewave-labs/loopgen-rs) | Rust | Agentic loop runner for Claude Code — compiles a goal into a structured harness and drives `claude -p` around a PLAN → ACT → VERIFY → REPORT cycle until a parsed `LOOP_STATUS` contract trips: `DONE` (optionally gated on a real verify command), `BLOCKED`, or a hard `--max` iteration cap |
| [secret-scan](https://github.com/adventurewave-labs/secret-scan) | Rust | Regex-based secret scanner for CI pipelines |
| [codescope](https://github.com/adventurewave-labs/codescope) | Rust | Single-binary code intelligence engine for AI coding agents — tree-sitter, MCP, CLI |
| [preflight-integration-tester](https://github.com/adventurewave-labs/preflight-integration-tester) | Python | Pre-deploy integration test harness |

#### In motion

<table>
  <tr>
    <td align="center" width="50%">
      <a href="https://github.com/adventurewave-labs/loopgen-rs"><img src="https://raw.githubusercontent.com/adventurewave-labs/loopgen-rs/main/demo.gif" width="420" alt="loopgen rendering an agentic loop harness with --dry-run"></a><br>
      <em>loopgen-rs — agentic loop runner</em>
    </td>
    <td align="center" width="50%">
      <a href="https://github.com/adventurewave-labs/codescope"><img src="https://raw.githubusercontent.com/adventurewave-labs/codescope/main/demo.gif" width="420" alt="codescope indexing itself and answering blast-radius queries"></a><br>
      <em>codescope — code intelligence for agents</em>
    </td>
  </tr>
  <tr>
    <td align="center">
      <a href="https://github.com/adventurewave-labs/secret-scan"><img src="https://raw.githubusercontent.com/adventurewave-labs/secret-scan/main/docs/secretscan-demo.gif" width="420" alt="secret-scan finding 6 planted secrets in a demo repo"></a><br>
      <em>secret-scan — CI secret scanner</em>
    </td>
    <td align="center">
      <a href="https://github.com/adventurewave-labs/preflight-integration-tester"><img src="https://raw.githubusercontent.com/adventurewave-labs/preflight-integration-tester/main/demo.gif" width="420" alt="preflight-integration-tester running a real readiness diagnostic — 97% GO, 3 middleware gaps found"></a><br>
      <em>preflight-integration-tester — AI readiness diagnostic</em>
    </td>
  </tr>
</table>

### Lab / Demos

Experiments, proofs of concept, and agentic demos.

| Repo | What it explores |
|---|---|
| [agentic-powered-golden-path-demo](https://github.com/adventurewave-labs/agentic-powered-golden-path-demo) | NL → GitOps deployment via golden-path workflows (ArgoCD + OpenRouter) |
| [AI-Kubernetes-API-Generator-Demo](https://github.com/adventurewave-labs/AI-Kubernetes-API-Generator-Demo) | NL → Kubernetes API generation |
| [agentic-devops-extravaganza](https://github.com/adventurewave-labs/agentic-devops-extravaganza) · [live demo](https://agentic-devops-extravaganza.vercel.app/) | Working demo of K8sGPT and Robusta running against a real Kubernetes API + GLM-4.5 LLM |
| [agentic-platform-engineering-extravaganza](https://github.com/adventurewave-labs/agentic-platform-engineering-extravaganza) · [live demo](https://agentic-platform-engineering-extravaganza.vercel.app/) | Golden path + Score → Crossplane + real OPA policy gates + an authz-gated MCP server — 42 policy violations without a platform, 0 with one |
| [aops-sre-pipeline](https://github.com/adventurewave-labs/aops-sre-pipeline) · [live demo](https://aops-sre-pipeline.vercel.app/) | Alert-driven autonomous SRE pipeline — Prometheus → n8n → Popeye → Dify-lite → Ollama → Slack |
| [gitops-progressive-delivery-demo](https://github.com/adventurewave-labs/gitops-progressive-delivery-demo) · [live demo](https://gitops-progressive-delivery-demo.vercel.app/) | Argo CD + Argo Rollouts + Prometheus + K8sGPT progressive delivery — a canary trips an SLO violation, an AI SRE diagnoses it, and the rollout auto-rolls back in ~20s |
| [moor](https://github.com/adventurewave-labs/moor) · [live demo](https://moor-devops-demo.vercel.app) | Desired-state control plane for docker-compose — OBSERVE → DIFF → PLAN → ACT drift detection with real auto-remediation against the live Docker Engine API ||
| [cloudtrim](https://github.com/adventurewave-labs/cloudtrim) · [live demo](https://cloud-trim-demo.vercel.app/) | 22-rule AWS cost-waste audit & remediation engine — read-only scan, verified fixes, and CUR-reconciled savings reporting demoed against a pinned AWS API emulator |

---

## FAQ

**What is Adventure Wave Labs?**
An open-source lab building developer tooling for the Claude and agentic AI ecosystem — CLIs, agentic loop runners, and code-intelligence tools used alongside Claude Code.

**What is Turbo-Flow?**
Turbo-Flow is Marcus Patman's open-source project (MIT). Versions 1–4 (2025–2026) were an agentic development environment — 215+ MCP tools, cross-session memory, per-agent git-worktree isolation. Since v5 it is the rules layer for AI-written code: rig-lite, a portable bash-only governance kit that works in any repo with any coding agent. See [marcuspat/turbo-flow](https://github.com/marcuspat/turbo-flow).

**Is this tooling used in production?**
The toolchain is dogfooded daily inside Turbo-Flow, and most repos have their own CI (see each repo's Actions badge). `preflight-integration-tester` is explicitly marked **pre-alpha** in its own README — it's a real, working tool, just not yet positioned as a production dependency for outside teams.

---

## Stack

Rust · Shell · Python · Claude Code · MCP · Kubernetes · Terraform

Founder-published crates on [crates.io](https://crates.io/users/marcuspat):

[![secretscan downloads](https://img.shields.io/crates/d/secretscan?label=secretscan)](https://crates.io/crates/secretscan) [![cargo-forge downloads](https://img.shields.io/crates/d/cargo-forge?label=cargo-forge)](https://crates.io/crates/cargo-forge) [![netrain downloads](https://img.shields.io/crates/d/netrain?label=netrain)](https://crates.io/crates/netrain) [![cargocrypt downloads](https://img.shields.io/crates/d/cargocrypt?label=cargocrypt)](https://crates.io/crates/cargocrypt) [![k8s-netinspect downloads](https://img.shields.io/crates/d/k8s-netinspect?label=k8s-netinspect)](https://crates.io/crates/k8s-netinspect) [![file-hasher downloads](https://img.shields.io/crates/d/file-hasher?label=file-hasher)](https://crates.io/crates/file-hasher)

---

<div align="center">

**Built & Presented by Adventure Wave Labs**

Built by [Marcus Patman](https://github.com/marcuspat) — Principal Agentic Engineer
LATAM AI solutions at [creandotumatrix-labs](https://github.com/creandotumatrix-labs)

📧 marcus@adventureonthewave.com · [adventurewavelabs.space](https://adventurewavelabs.space) · [LinkedIn](https://linkedin.com/in/marcuspatman) · [X @marcuspat](https://x.com/marcuspat) · [YouTube](https://youtube.com/@marcuspatmanagentics)

</div>
