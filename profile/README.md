# VESvault

**Real end-to-end encryption — with a way back in.**

VESvault gives developers true end-to-end encryption *and* a realistic recovery
path after a lost device — without the service ever being able to read your keys
or your data. New keys are **post-quantum by default** (ML-KEM / FIPS&nbsp;203).

### Why VES is different

- **Zero-knowledge server.** It stores only public keys, *encrypted* private
  keys, and *encrypted* vault entries. It never sees a VESkey or a decrypted
  private key — every decryption happens client-side.
- **Recovery without a backdoor.** Total device loss is handled by **threshold
  secret sharing** among recovery contacts you choose in advance (Shamir over
  GF(256), scheme `SSS1`). No single party — and no coalition of contacts —
  can recover your keys alone: each share is stored encrypted to its contact's
  key, so the server can't read any share; contacts never receive your
  encrypted keys; and recovery is time-delay protected and visible to the
  owner.
- **Open source.** The client libraries and the `ves` CLI are Apache-2.0.

### Projects

**Encryption libraries**

| | |
|---|---|
| 📦 **[libVES.c](https://github.com/vesvault/libVES.c)** | End-to-end encryption for data at rest — C library + `ves` CLI |
| 📦 **[libVES](https://github.com/vesvault/libVES)** | End-to-end encryption for the browser & Node — JavaScript (npm: `libves`) |
| 📝 **[VESpost](https://github.com/vesvault/vespost)** | Reference app — e2ee collaborative sticky notes in ~300 lines of `libVES.subtle` ([live demo](https://demo.ves.world), [walkthrough](https://dev.to/vesvaultjz/end-to-end-encrypted-collaborative-notes-in-300-lines-of-javascript-no-app-server-2mo)) |

**Apps & services**

| | |
|---|---|
| ✉️ **[VESmail](https://github.com/vesvault/VESmail)** | End-to-end encrypted email via a local proxy ([Android](https://github.com/vesvault/VESmail-android) · [Apple](https://github.com/vesvault/VESmail-apple) · [Windows](https://github.com/vesvault/VESmail-win)) |
| 🔐 **[VESlocker](https://veslocker.com)** | Hardware-grade PIN security API |
| 🌐 **[SNIF](https://github.com/vesvault/snif)** | End-to-end TLS trust for IoT |

### Docs & install

- 📖 **[Developer Center](https://ves.host)** — docs, specs, REST APIs
- 🌐 **[vesvault.com](https://www.vesvault.com)** — what is VES?
- 🍺 **[homebrew-ves](https://github.com/vesvault/homebrew-ves)** — `brew` tap for libVES.c & the VES CLI

### Community

Questions, integration help, ideas, and design scrutiny are all welcome in
**[Discussions](https://github.com/orgs/vesvault/discussions)**. We built VES to
be examined — hard questions about the threat model are exactly what we want.

> **Security issues:** please report vulnerabilities **privately** — see our
> [security policy](https://github.com/vesvault/.github/security/policy) —
> not in a public Discussion or issue.
