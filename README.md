# Hi, I'm Jesse

I build software in Wollongong: fast local AI on Intel Arc GPUs, planning tools, and a train game.

## Intel Arc + local AI
- **llama.cpp on Intel Arc (SYCL)**: XMX flash attention for quantized KV caches (up to 2.6x faster generation at long context on a B580), XMX prompt GEMMs for the default fp32 build (~3x faster prompt processing), and a faster GATED_DELTA_NET kernel for Qwen3.5-style models. Sent to Intel's SYCL maintainer for upstreaming. Branches: [sycl-fa-q4-xmx](https://github.com/Torchit1/llama.cpp/tree/sycl-fa-q4-xmx), [sycl-xmx-prompt-gemm](https://github.com/Torchit1/llama.cpp/tree/sycl-xmx-prompt-gemm), [sycl-gdn-blocked](https://github.com/Torchit1/llama.cpp/tree/sycl-gdn-blocked)
- **[Bonsai 2 27B on Intel Arc B580](https://github.com/Torchit1/llama.cpp/tree/arc-b580)**: SYCL kernels that run PrismML's ternary 27B model on a 12 GB Arc B580 with the full 128K context, ~85 t/s with speculative decoding.
- **[TernSYCL](https://github.com/libxsmm/TernSYCL)** (contributor, 4 merged PRs): int4/int8 DPAS helpers and fixes for ternary GEMM kernels on Xe GPUs.
- **[wayfinder](https://github.com/Torchit1/wayfinder)**: lets an AI agent point at things on your Windows screen instead of clicking for you.

## Other projects
- **[Next Stop NSW](https://nextstopnsw.com.au)**: a browser train game built on the real NSW rail network.
- **[AusDatum](https://ausdatum.com.au)**: NSW site and planning analysis: zoning, hazards and development pathways for any lot.
- **[PyAtlasPro](https://github.com/Torchit1/PyAtlasPro)**: a free pyRevit extension for faster Revit drafting.

Best way to reach me is [LinkedIn](https://www.linkedin.com/in/jessesymons/).
