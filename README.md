# GPU Architecture Visualization

Interactive single-page visualization of NVIDIA GPU architectures, combining the **hardware floorplan** (GPC / TPC / SM, L2, HBM) with the **software execution model** (Grid / Cluster / Block / Warp / Thread) and the **memory hierarchy** (Registers / SMEM / L1 / L2 / GMEM).

Switchable GPUs: **V100** (Volta), **A100** (Ampere), **H100** (Hopper), **RTX 4090** (Ada), **B100** & **B200** (Blackwell).

## Features

- Die floorplan with accurate GPC × TPC × SM counts and real-world binning patterns per SKU
- Click-/hover-driven SM expansion showing a 1-cycle pipeline: Warp Scheduler → Dispatch → Execution Units → Register File
- SM-level resident warp pool (max 64 warp × 32 = 2048 thread, partitioned 4 ways)
- Cluster + DSMEM (Hopper+) shown only where the architecture supports it
- Nested SW ↔ HW stack with each level's memory + compute resources
- Light / Dark / Auto theme

Pure static HTML / CSS / JS — no build step, no dependencies.

## Local

Just open `index.html` in a browser.

## License

MIT
