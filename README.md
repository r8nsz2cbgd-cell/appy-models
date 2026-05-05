# appy-models

On-device AI model assets for [AppyPilgrim](https://appypilgrim.it).

GGUFs are attached to GitHub Releases — see the **Releases** tab.

## Why not HuggingFace?

HF auto-migrated our repos to their Xet CDN (`cas-bridge.xethub.hf.co`),
which serves files via AWS-signed S3 redirects with 1300+ character
URLs. iOS `URLSessionConfiguration.background` does not follow those
redirects reliably and stalls or times out on real devices. GitHub
Releases redirects are simple (`releases/download/...` → `objects.
githubusercontent.com`) and iOS BG URLSession handles them cleanly.

Models are also on HuggingFace at
[Valerio81/appy-1b-v5-gguf](https://huggingface.co/Valerio81/appy-1b-v5-gguf)
and
[Valerio81/appy-qwen25-1b5-gguf](https://huggingface.co/Valerio81/appy-qwen25-1b5-gguf)
for non-iOS clients.
