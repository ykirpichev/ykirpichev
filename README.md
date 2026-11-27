LLM training, serving, and GPU kernels, measured and written up so each result can be rerun.
Everything is in one place at **[ykirpichev.github.io](https://ykirpichev.github.io/)**.

**Book:** [Engineering Large Language Models](https://ykirpichev.github.io/llm-book-site/). Free, 68 chapters on training, inference, kernels, and distributed systems. [PDF](https://ykirpichev.github.io/llm-book-site/engineering-large-language-models.pdf)

| Study | Result |
|---|---|
| [Multi-teacher on-policy distillation on TPU v6e](https://ykirpichev.github.io/mopd-tpu/) | 17.4% vs 14.0% AIME pass@1 against mixed-reward RL |
| [Async vs sync RL rollouts on TPU v6e](https://ykirpichev.github.io/async-vs-sync-rl-tpu/) | 1.72× faster per step than sync, no loss of accuracy |
| [TPU v6e vs H100 serving](https://ykirpichev.github.io/tpu-vs-h100-llm-bench/) | $0.90 vs $2.54 per million output tokens (Cosmos3-Super) |
| [Cosmos 3 vs Cosmos 2 vs Qwen on lane behavior](https://github.com/ykirpichev/cosmos-reason2-lane-eval/blob/main/docs/summary_report.md) | 0.93 vs 0.74 vs 0.69 accuracy |
| [Sparse attention kernels, MLSys 2026 contest](https://github.com/ykirpichev/dsa_topk_indexer_fp8_h64_d128_topk2048_ps64/blob/main/final_writeup.md) | 28.96× over the FlashInfer baselines on B200 |
| One kernel in four languages: [top-K indexer](https://ykirpichev.github.io/dsa_topk_indexer_fp8_h64_d128_topk2048_ps64/frameworks/), [sparse attention](https://ykirpichev.github.io/dsa_sparse_attention_h16_ckv512_kpe64_topk2048_ps64/frameworks/) | CUDA, Triton, TileLang, and ThunderKittens on B200 |

Corrections welcome: open an issue on the study's repository. [LinkedIn](https://www.linkedin.com/in/ykirpichev/)
