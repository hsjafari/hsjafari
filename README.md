# hsjafari

Red Team Operator & Python toolsmith. I build adversary-emulation tooling, C2 bits, and automation that doesn’t wake you up at 03:00.  
*aka R0n1n*

[![Follow](https://img.shields.io/github/followers/hsjafari?label=Follow&style=social)](https://github.com/hsjafari)
[![Stars](https://img.shields.io/github/stars/hsjafari?affiliations=OWNER%2CCOLLABORATOR&style=social)](https://github.com/hsjafari?tab=repositories)

---

## What I build
- **C2 & operator tools**: tasking, op logs, opsec guardrails, repeatable flows.
- **Loaders & implants**: staged/stageless, selective telemetry, quiet comms.
- **Tradecraft automation**: recon → initial access → privilege → persistence → exfil.
- **Research**: EDR/telemetry evasion, behavioral shaping, sandbox dodging.

## Focus areas
`adversary emulation` · `OPSEC-first engineering` · `EDR bypass R&D` · `Windows internals` · `network tradecraft` · `operator ergonomics`

## Stack
**Python** (asyncio, uvloop, ctypes, pycryptodome)  
**C** (minimal stubs/shims), **Bash**, a pinch of **PowerShell**  
Packagers/Build: `PyInstaller` · `Nuitka` · `CMake`  
Infra: `Flask/FastAPI` · `Redis` · `SQLite/Postgres` · `Docker`  
Protocols: `HTTP(S)` · `DNS` · `WebSocket` · `Named Pipes`  

## Currently
- Hardening a Python C2 core (transport abstractions + opsec checks).
- Prototyping a loader chain with staged AES-GCM and in-memory exec.
- Writing tests that catch the “works on my box” lies.

## Ethos
Only for **authorized** engagements and research. If you’re not the owner or don’t have written permission, don’t touch it.

---

### Selected repos
> Pin your top projects so they surface here.
- 🔴 **cortex-c2** — operator-first Python C2 with transport plugins.
- 🧬 **cortex-loader** — staged/reflective loaders (Python/C interop).
- 🛰️ **cortex-kits** — repeatable tradecraft automations and op checklists.
- 🧪 **cortex-labs** — small R&D drops (EDR tests, evasion PoCs).

*(Rename links above to your actual repos once public.)*

---

## Quick start (for most projects)
```bash
python -m venv .venv && source .venv/bin/activate
pip install -U pip wheel
pip install -r requirements.txt
pytest -q
