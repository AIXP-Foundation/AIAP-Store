<!-- markdownlint-disable MD041 -->
<div align="center">
  <h1>AIAP Store</h1>
  <p><b>The official marketplace for AIAP programs — discover, publish, and distribute AI capabilities.</b></p>
  <p>
    <a href="https://aiap.dev"><img src="https://img.shields.io/badge/Protocol-AIAP_V1.0.0-brightgreen.svg" alt="AIAP V1.0.0" /></a>
    <a href="https://aiap.store"><img src="https://img.shields.io/badge/docs-aiap.store-blue.svg" alt="Docs" /></a>
  </p>
  <p>
    <a href="README_CN.md">中文文档</a> | English
  </p>
</div>

## What is AIAP Store?

AIAP Store is the central distribution platform for **AIAP programs** — AI capability packages that conform to the [AIAP Protocol](https://github.com/AIXP-Foundation/AIAP). It serves the same role for AI programs that npm serves for JavaScript packages or Docker Hub serves for container images.

Every program on AIAP Store is:

- **Structurally verified** — passes AIAP protocol validation
- **Quality-scored** — evaluated by ThreeDimTest (Correctness, Intrinsic, Detail)
- **License-declared** — SPDX-compliant license field required (PL25)
- **Governance-signed** — SHA-256 governance hash for integrity verification

---

## What is an AIAP Program?

An AIAP program (`*_aiap/`) is a structured AI capability package:

```
my_program_aiap/
├── AIAP.md            # Governance contract (identity, tools, trust level, license)
├── main.aisop.json    # Entry point with Mermaid or JSON flow execution graph
└── module.aisop.json  # Functional module
```

Programs are created with [AIAP Creator](https://soulbot.dev) and run on the [SoulBot](https://soulbot.dev) runtime.

---

## Store Requirements

To publish a program on AIAP Store, it must:

| Requirement | Rule | Details |
|-------------|------|---------|
| Protocol compliance | MF1 | Valid `AIAP.md` governance contract |
| Quality threshold | ThreeDimTest | Minimum passing score |
| License declared | PL25 | Each program must declare its own SPDX license — AIAP Store does not impose a platform license |
| Governance hash | MF15 | SHA-256 integrity verification |
| Trust level declared | T1-T4 | Appropriate trust boundary |

---

## AIXP Foundation [www.aixp.dev](https://aixp.dev)

The AIXP Foundation develops and maintains the following core projects:

| Project | Description | Website |
|---------|-------------|---------|
| [HSAW](https://hsaw.dev) | Human Sovereignty and Wellbeing — Axiom 0 white paper (foundation) | hsaw.dev |
| [AILP](https://ailp.dev) | AI List Protocol — agent discovery and capability advertising | ailp.dev |
| [AIVP](https://aivp.dev) | AI Value Protocol — international commerce, crypto asset settlement | aivp.dev |
| [AIRP](https://airp.dev) | AI RMB Protocol — Mainland China commerce, RMB licensed settlement | airp.dev |
| [AIBP](https://aibp.dev) | AI Bot Protocol — social communication and trust | aibp.dev |
| [AIAP](https://aiap.dev) | AI Application Protocol — governance and compliance | aiap.dev |
| [AISOP](https://aisop.dev) | AI Standard Operating Protocol — flow program definition | aisop.dev |
| [SoulBot](https://soulbot.dev) | AI agent runtime and framework | soulbot.dev |
| [SoulACP](https://soulacp.dev) | Adapter library — bridging CLI tools and LLM providers | soulacp.dev |

---

## Status

AIAP Store is currently under development. Follow this repository to be notified when it launches.

- [ ] Store API specification
- [ ] Program submission portal
- [ ] Quality gate CI/CD pipeline
- [ ] Search and discovery interface
- [ ] Author verification system

---

## License

AIAP Store is a distribution platform. **Each AIAP program carries its own license**, declared via the `license` field in its `AIAP.md` governance contract (rule PL25). The Store platform code itself does not impose a license on hosted programs.

---

Align Axiom 0: Human Sovereignty and Wellbeing. Version: AIAP V1.0.0. www.aiap.store
