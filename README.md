# Awesome-Multimodal-Reasoning

**Contributions are most welcome**, if you have any suggestions or improvements, feel free to create an issue or raise a pull request.

## Contents
 - [Benchmark](#Visual-Reasoning-Benchmark)
 - [Supervised Fine-Tuning](#Supervised-Fine-Tuning)
 - [Reinforcement Learining](#Reinforcement-Learining)
 - [SFT + RL](##SFT+RL)



## TODO

[https://arxiv.org/pdf/2503.07365](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/2503.07365)
标题：[MM-Eureka](https://zhida.zhihu.com/search?content_id=254920452&content_type=Article&match_order=1&q=MM-Eureka&zhida_source=entity): Exploring Visual Aha Moment with Rule-based Large-scale Reinforcement Learning
关键词：RL, reasoning model
简介：作者提出了MM-Eureka，一个多模态reasoning model

[https://arxiv.org/pdf/2503.06749](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/2503.06749)
标题： Vision-R1: Incentivizing Reasoning Capability in Multimodal Large Language Models
关键词：RL, reasoning model, MLLM
简介：作者探究了如何通过RL来提升MLLM的reasoning能力

[https://arxiv.org/pdf/2503.07065](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/2503.07065)
标题：Boosting the Generalization and Reasoning of Vision Language Models with Curriculum Reinforcement Learning
关键词：RL, curriculum learning, reasoning
简介：作者提出了CurrReFT，一个提升小VLM的reasoning能力和OOD泛化能力的post-training方法

[https://arxiv.org/pdf/2503.07523](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/2503.07523)
标题：[VisRL](https://zhida.zhihu.com/search?content_id=254920452&content_type=Article&match_order=1&q=VisRL&zhida_source=entity): Intention-Driven Visual Perception via Reinforced Reasoning
关键词：RL, visual perception, reasoning
简介：作者提出了VisRL，一个从task feedback中学习intention-driven visual perception的框架

[https://arxiv.org/pdf/2503.06514](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/2503.06514)
标题：[GFlowVLM](https://zhida.zhihu.com/search?content_id=254920452&content_type=Article&match_order=1&q=GFlowVLM&zhida_source=entity): Enhancing Multi-step Reasoning in Vision-Language Models with Generative Flow Networks
关键词：VLM, multi-step reasoning
简介：作者提出了GFlowVLM，一个用于提升VLM多步推理能力的框架

[https://arxiv.org/pdf/2503.07536](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/2503.07536)
标题：LMM-R1: Empowering 3B LMMs with Strong Reasoning Abilities Through Two-Stage Rule-Based RL
关键词：RL, LMM, reasoning
简介：作者提出了LMM-R1，一个用于提升LMM的reasoning能力的两阶段框架

## Multimodal Reasoning Benchmark

- [**M**3**CoT: A Novel Benchmark for Multi-Domain Multi-step Multi-modal Chain-of-Thought**](https://arxiv.org/html/2405.16473v1)
- [MME-CoT 🔥🕵️: Benchmarking Chain-of-Thought in LMMs for Reasoning Quality, Robustness, and Efficiency](https://github.com/CaraJ7/MME-CoT)

## Supervised Fine-Tuning
### Image MLLM
- [Virgo: A Preliminary Exploration on Reproducing o1-like MLLM](https://arxiv.org/abs/2501.01904)
- [LLaVA-CoT: Let Vision Language Models Reason Step-by-Step](https://arxiv.org/abs/2411.10440)
### Video MLLM

## Reinforcement Learining

### Image MLLM

| Date  | Project                                                      | Comment |
| ----- | ------------------------------------------------------------ | ------- |
| 25.01 | InternLM-XComposer2.5-Reward: A Simple Yet Effective Multi-Modal Reward Model [[Paper]](https://arxiv.org/abs/2501.12368) [[Code]]() |         |
| 24.11 | Enhancing the Reasoning Ability of Multimodal Large Language Models via Mixed Preference Optimization [[Paper]](https://arxiv.org/abs/2411.10442) [[Code]()] |         |
| 25.02 | MM-RLHF: The Next Step Forward in Multimodal LLM Alignment [[Paper]](https://arxiv.org/abs/2502.10391) |         |
|       | OmniAlign-V: Towards Enhanced Alignment of MLLMs with Human Preference [[Code]](https://github.com/PhoenixZ810/OmniAlign-V) |         |
|       | VLM-R1 [[Code]](https://github.com/om-ai-lab/VLM-R1/tree/main?tab=readme-ov-file) |         |
| 25.03 | Unified Reward Model for Multimodal Understanding and Generation [[Paper]](https://arxiv.org/abs/2503.05236) |         |
|       | MM-EUREKA: Exploring Visual Aha Moment with Rule-based Large-scale Reinforcement Learning [[Code]](https://github.com/ModalMinds/MM-EUREKA) |         |
| 25.03 | R1-Zero’s “Aha Moment” in Visual Reasoning on a 2B Non-SFT Model [[Paper]](https://arxiv.org/abs/2503.05132) |         |
|       | Seg-Zero: Reasoning-Chain Guided Segmentation via Cognitive Reinforcement [[Code]](https://github.com/dvlab-research/Seg-Zero) |         |
| 25.03 | Vision-R1: Incentivizing Reasoning Capability in Multimodal Large Language Models [[Paper]](https://arxiv.org/abs/2503.06749) |         |



### Video MLLM

| Date | Project                                                      | Comment |
| ---- | ------------------------------------------------------------ | ------- |
|      | Open-R1-Video[[Code]](https://github.com/Wang-Xiaodong1899/Open-R1-Video) |         |
|      | Video-R1[[Code]](https://github.com/tulerfeng/Video-R1)      |         |
|      | Temporal Preference Optimization for Long-Form Video Understanding [[Paper]](https://arxiv.org/abs/2501.13919) |         |



### Image Generation

TODO

## SFT+RL

### Image MLLM
- [Improve Vision Language Model Chain-of-thought Reasoning](https://arxiv.org/pdf/2410.16198)

### Video MLLM
- [Tarsier2: Advancing Large Vision-Language Models from Detailed Video Description to Comprehensive Video Understanding]()
- [video-SALMONN-o1: Reasoning-enhanced Audio-visual Large Language Model](https://arxiv.org/abs/2502.11775)



## Other

[Multimodal Chain-of-Thought Reasoning in Language Models](https://github.com/amazon-science/mm-cot)
