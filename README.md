# Quantum
Physical Quantum Mechanic
# Nirun OS Quantum Edition

**A quantum-inspired, bootable operating system with a 3D volumetric desktop — built for education, research, and experimentation on everyday hardware.**

Nirun OS is **not** a real quantum computer OS. It is a **classical OS** that simulates quantum-inspired concepts (voxel lattices, topological analogies, error-correcting heuristics, neural acceleration) in a visually intuitive 3D environment.

It runs on ordinary x86 PCs (via QEMU or bare metal), Docker, and soon ARM/Raspberry Pi — no cryogenic cooling, no cloud subscription, no expensive QPU required.

## Vision

Make quantum ideas feel accessible and tangible for everyone — students, researchers, developers, and enthusiasts — through a beautiful 3D desktop where "quantum" behaviors (healing, diffusion, raycasting) happen in real time.

One man, one mission, one OS to rule them all.

## Current Status (v1.4.0-docker — February 2026)

- Bootable monolithic kernel (Multiboot, i386)
- 20 Hz real-time scheduler (PIT-driven)
- 4×4×4 toroidal voxel lattice (DR9 invariant + E9P 26-neighbor healing)
- Thermal entropy diffusion model
- Isometric 3D volumetric window manager (VGA Mode 13h)
- Neural Raycast engine (LibTorch C++ inference — GPU 0.052 ms / CPU 0.18 ms, 95%+ acc)
- Grok semantic bridge (mock → real API ready)
- Full Docker pipeline + GitHub Actions CI/CD (Trivy clean)
- Documentation suite (specification, architecture diagrams, build guides)

## Key Features

- **Kernel**: Multiboot, GDT/IDT, PIT timer, basic memory manager
- **DR9 Core**: 4×4×4 toroidal lattice with invariant check ((x+y+z) mod 9 = 0)
- **E9P Healing**: 26-neighbor majority voting for auto-correction
- **Thermal Model**: Entropy diffusion simulation (Eq. 14)
- **3D GUI**: Isometric voxel renderer, window creation/movement/z-order
- **Neural Raycast**: LibTorch-based inference with CUDA/CPU fallback (80% octree reduction at high confidence)
- **Quantum Bridge**: Grover decoder simulation + QEC controller (20 Hz closed-loop)
- **Deployment**: Multi-stage Docker (312 MB), QEMU profiles, GitHub CI/CD

## Quick Start (Recommended: Docker)

```bash
# Build locally
docker build -t nirun-os .

# Run interactive shell inside container
docker run --rm -it nirun-os

# Or boot the ISO in QEMU (after make build_iso)
qemu-system-i386 -cdrom build/iso/NirunOS-Quantum-v1.4.iso -m 512M -vga std
```

See `docs/build_and_run_guide.md` for full instructions, troubleshooting, and hardware notes.

## Contributing

We warmly welcome contributors of all skill levels — from documentation, translation, testing, to kernel/GUI development.

1. Read our [Contributing Guide](./CONTRIBUTING.md)
2. Browse **good first issues**: https://github.com/SiriRangsanTech/Quantum/labels/good-first-issue
3. Fork → create branch → commit → pull request
4. Join the conversation on **Discord** (invite link coming soon)

We follow the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/).

## Community & Communication

- **Discord** — Primary chat & sync (invite link to be added)
- **GitHub Discussions** — https://github.com/SiriRangsanTech/Quantum/discussions
- **X / Twitter** — @SiriRangsanTech for updates
- **Telegram** — Backup announcements (link to be added)

## License

Apache-2.0 (see [LICENSE](./LICENSE))

## Citation (for academic / thesis use)

If you use Nirun OS in research, publications, or a thesis, please cite:

```bibtex
@misc{nirun-os-2026,
  author       = {Rangsan Petkong (Commander Ω)},
  title        = {Nirun OS Quantum Edition},
  year         = {2026},
  publisher    = {GitHub},
  journal      = {GitHub repository},
  howpublished = {\url{https://github.com/SiriRangsanTech/Quantum}},
}
```

Thank you for joining the journey.  
Let's build the future of intuitive, quantum-inspired computing together!

— Commander Ω & the Nirun OS Community 🚀🧠![Uploading 1000306422.jpg…]()
