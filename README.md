# Momin Aldahdouh

15 · Tampere, Finland · CTO & Co-founder @ [MowisAI](https://mowisai.com)

Self-taught since 12. I build systems — not apps that wrap APIs.  
Currently: AI agent infrastructure in Rust. Previously: OS dev in NASM/C.

---

## MowisAI

> On-premises AI agent infrastructure. Run thousands of isolated agents in parallel on your own hardware.

Most agent frameworks coordinate. Most sandboxes execute. MowisAI does both — on your infrastructure, not ours.

**Core engine** (`mowisai` binary):
- Overlayfs/chroot/cgroups sandboxing — each agent gets an isolated filesystem layer
- Unix socket server with JSON-RPC protocol
- 75 built-in tools across 14 categories
- 7-layer orchestration: planner → hub agents → workers, event-driven scheduling
- 67 tests passing, clean `cargo build`

**Stack:** Rust · Linux kernel APIs · overlayfs · cgroups · Vertex AI Gemini 2.5 Pro · GCP  
**Target:** Developers and enterprises that need massive, complex agent workflows — fully sovereign.

→ [github.com/Momin010/MowisAI](https://github.com/Momin010/MowisAI) · [mowisai.com](https://mowisai.com)

---

## MominOS

> 64-bit x86_64 OS built from scratch in assembly — real mode to long mode.

Transitions from 16-bit Real Mode through GDT and 4-level paging into 64-bit Long Mode. Micro-kernel with a working interactive shell.

**What's implemented:**
- Stage 1 MBR bootloader + Stage 2 loader (A20, GDT, paging, long mode jump)
- 64-bit micro-kernel with full IDT — all 32 CPU exceptions handled
- Scrolling VGA driver + keyboard driver
- Functional CLI shell

**Stack:** NASM · QEMU · Assembly (89%) · x86_64

→ [github.com/Momin010/MominOS](https://github.com/Momin010/MominOS)

---

## Stack

**Systems:** Rust · C · NASM Assembly · Linux internals  
**Web/App:** TypeScript · React · Node.js · Supabase  
**Infra:** GCP · Vercel · overlayfs · cgroups · Unix sockets  

---

## Contact

[momin.aldahdooh@mowisai.com](mailto:momin.aldahdooh@mowisai.com) · [mowisai.com](https://mowisai.com)
