### Turboquant Implementation
- Google Research의 TurboQuant (arXiv:2504.19874) 논문을 PyTorch로 구현한 프로젝트입니다.
- [Source repository here] (https://github.com/javafa/turboquant)

**Baseline(FP16) 대비 비교:**

| 구성 | VRAM | KV Cache | 속도 (short) | 속도 (long) |
|---|---|---|---|---|
| BnB 4-bit | **-53.5%** | 동일 | -28.6% | -37.3% |
| TurboQuant 3-bit | 동일 | **-39.9%** | **+23.1%** | **+5.3%** |
| BnB 4-bit + TurboQuant | **-53.5%** | **-39.9%** | -29.4% | -38.5% |
| Unsloth 4-bit | -42% | 동일 | -41.1% | -17.5% |
| Unsloth 4-bit + TurboQuant | -42% | **-39.9%** | -5.5% | -12.7% |

### Ranked 1st on the huggingface Open Llm Leaderboard
- This is a merged model. So you have to unckeck the "[X] Contains merge/moerge" checkbox above the list.

|             Metric              |Value|
|---------------------------------|----:|
|Avg.                             |81.28|

### free-evo-qwen72b-v0.8
- [model repository here](https://huggingface.co/freewheelin/free-evo-qwen72b-v0.8-re)   

