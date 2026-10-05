<div align="center">

# jeryd (@UberMetroid)

**Systems Programmer & Open Source Architect**

Building capability-secure runtimes, verifiable supply-chain tooling, and native Linux OS primitives.

[Website](https://ubermetroid.github.io) • [studio2201](https://studio2201.com) • [openOODA](https://openooda.org) • [syntropd](https://syntropd.github.io) • [IdleScreen](https://idlescreen.github.io)

---

</div>

## Organizations & Ecosystems

### [openOODA](https://github.com/openOODA) · [openooda.org](https://openooda.org)
> **Capability-secure systems programming language.**
- Every external effect requires an explicit, unforgeable capability token — fail-closed by design.
- Merkle-AST cached compiler (`oodac`), capability runtime (`oodar`), package manager (`opm`), standard library (`std`), and agent flight recorder (`bb`).
- Ecosystem of capability-bounded POSIX replacements in [openOODA-tools](https://github.com/openOODA-tools) (`oogrep`, `oojq`, `oofind`, `oodiff`, `ootail`, `oosh`).

### [studio2201](https://github.com/studio2201) · [studio2201.com](https://studio2201.com)
> **Post-2030 software supply chain governance and attestation.**
- Five Apache-2.0 auditing tools built with **pure `std::` Rust** (0 crates from crates.io) and strictly **&le; 256 LOC per file**:
  - [**Snip**](https://github.com/studio2201/snip): Vibe-code, secrets, and PII static analyzer for LLM-generated diffs.
  - [**Vigil**](https://github.com/studio2201/vigil): Dependency dormancy and unmaintained library scanner across npm, cargo, and pip.
  - [**Aegis**](https://github.com/studio2201/aegis): NIST Post-Quantum Cryptography (PQC) migration scanner flagging deprecated RSA call sites.
  - [**Proven**](https://github.com/studio2201/proven): SLSA L3+ attestation engine signed with pure std ML-DSA-65.
  - [**Boneyard**](https://github.com/studio2201/boneyard): Repository health scoring and dormant public asset radar.

### [syntropd](https://github.com/syntropd) · [syntropd.github.io](https://syntropd.github.io)
> **Native AI Subsystem for systemd Linux.**
- Bakes local AI acceleration, demand-paged inference, and autonomous fault remediation directly into Linux as systemd native units and Varlink services.
- Decoupled daemon architecture: [`runtimed`](https://github.com/syntropd/runtimed), [`modeld`](https://github.com/syntropd/modeld), [`inferenced`](https://github.com/syntropd/inferenced), [`contextd`](https://github.com/syntropd/contextd), [`toold`](https://github.com/syntropd/toold), [`routerd`](https://github.com/syntropd/routerd), [`sentry`](https://github.com/syntropd/sentry), and unified CLI [`syntropctl`](https://github.com/syntropd/syntropctl).

### [IdleScreen](https://github.com/idlescreen) · [idlescreen.github.io](https://idlescreen.github.io)
> **Wayland-native ambient display and screensaver suite.**
- Modular Linux idle screensaver daemon with D-Bus IPC, plugin sandbox host, 11 procedural visualizers, COSMIC desktop applet, and APT/RPM packaging channel.

---

## Notable Projects & Tools

| Project | Description | Tech Stack |
| :--- | :--- | :--- |
| [**glances-rs**](https://github.com/UberMetroid/glances-rs) | Zero-dependency Linux system monitor in one static binary. Full REST, SSE, XML-RPC, MCP, CSV, JSON surfaces and 18 exporters. | Pure Rust `std::` |
| [**necrometer**](https://github.com/necrometer-dev/necrometer) | Measures how dead your GitHub repositories are. Embeddable necrosis badges and cards. | Rust, WebAssembly, SVG |
| [**ahamkara**](https://github.com/UberMetroid/ahamkara) | Canonical archive and Rust query engine for the Ahamkara wish-dragons of Destiny. | Rust, TypeScript, Pages |
| [**beatniks-bumtrips-bullshit**](https://github.com/bumtrips/beatniks-bumtrips-bullshit) | Audio archive and field recordings exploring literature and counterculture. | Static Web, Audio |

---

## Engineering Constitution

1. **Pure Standard Library**: Favor zero-dependency architectures (`std::` only) where attack surfaces and supply-chain hygiene matter.
2. **Explicit Capabilities**: Zero ambient authority; all side-effects must carry verifiable capability tokens.
3. **Strict Bounds & Locality**: Maintain disciplined line-of-code budgets (&le; 256 LOC per file) to prevent architectural rot and keep code human- and agent-comprehensible.
4. **Deterministic & Verifiable**: Bit-for-bit reproducible builds, cryptographic provenance attestations, and formal verification gates.
