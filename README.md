# Awesome-Multimodal-Reasoning

**Contributions are most welcome**, if you have any suggestions or improvements, feel free to create an issue or raise a pull request.

## Contents
 - [Benchmark](##Benchmark)
 - [Model](##Model)
 - [Data](##Data)

## Benchmark



| Date  | Project                                                      | Task          |
| ----- | ------------------------------------------------------------ | ------------- |
| 24.05 | M3CoT: A Novel Benchmark for Multi-Domain Multi-step Multi-modal Chain-of-Thought [[Paper]](https://arxiv.org/html/2405.16473v1) | M3CoT         |
| 24.10 | MME-CoT: Benchmarking Chain-of-Thought in LMMs for Reasoning Quality, Robustness, and Efficiency [[Paper]](https://arxiv.org/pdf/2410.16198)[[Code]](https://github.com/CaraJ7/MME-CoT) | MME-CoT       |
| 25.02 | OmniAlign-V: Towards Enhanced Alignment of MLLMs with Human Preference [[Paper]](https://arxiv.org/abs/2502.18411)[[Code]](https://github.com/PhoenixZ810/OmniAlign-V) | MM-AlignBench |
| 24.11 | VLRewardBench: A Challenging Benchmark for Vision-Language Generative Reward Models [[Paper]](https://arxiv.org/abs/2411.17451) | VLRewardBench                            |
| 25.02 | MM-RLHF: The Next Step Forward in Multimodal LLM Alignment [[Paper]](https://arxiv.org/abs/2502.10391) | MM-RLHF-RewardBench, MM-RLHF-SafetyBench |

## Model

### Image MLLM

| Date  | Project                                                      | SFT                                                  | RL   | Task                                                         |
| ----- | ------------------------------------------------------------ | ---------------------------------------------------- | ---- | ------------------------------------------------------------ |
| 24.10 | Improve Vision Language Model Chain-of-thought Reasoning [[Paper]](https://arxiv.org/pdf/2410.16198)[[Code]](https://github.com/RifleZhang/LLaVA-Reasoner-DPO) | 193k CoT sft data by GPT4-o                          | DPO  | Various VQA                                                  |
| 24.11 | LLaVA-CoT: Let Vision Language Models Reason Step-by-Step [[Paper]](https://arxiv.org/abs/2411.10440)[[Code]](https://github.com/PKU-YuanGroup/LLaVA-CoT) | LLaVA-CoT-100k by GPT4-o                             | -    | Various VQA                                                  |
| 24.11 | Enhancing the Reasoning Ability of Multimodal Large Language Models via Mixed Preference Optimization [[Paper]](https://arxiv.org/abs/2411.10442) | -                                                    | MPO  | Various VQA                                                  |
| 25.01 | Virgo: A Preliminary Exploration on Reproducing o1-like MLLM [[Paper]](https://arxiv.org/abs/2501.01904)[[Code]](https://github.com/RUCAIBox/Virgo) | 2k Text data from R1/QwQ and visual data from QvQ/SD | -    | Math & MMMU                                                  |
| 25.01 | InternLM-XComposer2.5-Reward: A Simple Yet Effective Multi-Modal Reward Model [[Paper]](https://arxiv.org/abs/2501.12368)[[Code]](https://github.com/InternLM/InternLM-XComposer) | -                                                    | PPO  | Reward & Various VQA                                         |
| 25.02 | MM-RLHF: The Next Step Forward in Multimodal LLM Alignment [[Paper]](https://arxiv.org/abs/2502.10391) | -                                                    | DPO  | Reward & Various VQA                                         |
| 25.02 | OmniAlign-V: Towards Enhanced Alignment of MLLMs with Human Preference [[Paper]](https://arxiv.org/abs/2502.18411)[[Code]](https://github.com/PhoenixZ810/OmniAlign-V) | 200k sft data                                        | DPO  | Alignment & Various VQA                                      |
| 25.02 | VLM-R1: A stable and generalizable R1-style Large Vision-Language Model [[Code]](https://github.com/om-ai-lab/VLM-R1/tree/main?tab=readme-ov-file) | -                                                    | GRPO | Referring Expression Comprehension                           |
| 25.02 | R1-V: Reinforcing Super Generalization Ability in Vision Language Models with Less Than $3 [[Code]](https://github.com/Deep-Agent/R1-V) | -                                                    | GRPO | Item Counting, Number Related Reasoning and Geometry Reasoning |
| 25.03 | Unified Reward Model for Multimodal Understanding and Generation [[Paper]](https://arxiv.org/abs/2503.05236)[[Code]](https://codegoat24.github.io/UnifiedReward/) | -                                                    | DPO  | Various VQA & Generation                                     |
| 25.03 | MM-EUREKA: Exploring Visual Aha Moment with Rule-based Large-scale Reinforcement Learning [[Paper]](https://arxiv.org/abs/2503.07365)[[Code]](https://github.com/ModalMinds/MM-EUREKA) |                                                      |      |                                                              |
| 25.03 | R1-Zero’s “Aha Moment” in Visual Reasoning on a 2B Non-SFT Model [[Paper]](https://arxiv.org/abs/2503.05132) |                                                      |      |                                                              |
|       | Seg-Zero: Reasoning-Chain Guided Segmentation via Cognitive Reinforcement [[Code]](https://github.com/dvlab-research/Seg-Zero) |                                                      |      |                                                              |
| 25.03 | Vision-R1: Incentivizing Reasoning Capability in Multimodal Large Language Models [[Paper]](https://arxiv.org/abs/2503.06749) |                                                      |      |                                                              |
| 25.03 | Boosting the Generalization and Reasoning of Vision Language Models with Curriculum Reinforcement Learning [[Paper]](https://arxiv.org/pdf/2503.07065) |                                                      |      |                                                              |
| 25.03 | LMM-R1: Empowering 3B LMMs with Strong Reasoning Abilities Through Two-Stage Rule-Based RL [[Paper]](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/2503.07536) |                                                      |      |                                                              |
| 25.03 | VisRL: Intention-Driven Visual Perception via Reinforced Reasoning [[Paper]](https://arxiv.org/pdf/2503.07523) |                                                      |      |                                                              |
| 25.03 | GFlowVLM: Enhancing Multi-step Reasoning in Vision-Language Models with Generative Flow Networks [[Paper]](https://arxiv.org/pdf/2503.06514) |                                                      |      |                                                              |



### Video MLLM

| Date  | Project                                                      | SFT  | RL   | Comment |
| ----- | ------------------------------------------------------------ | ---- | ---- | ------- |
|       | Open-R1-Video[[Code]](https://github.com/Wang-Xiaodong1899/Open-R1-Video) |      | GRPO |         |
|       | Video-R1[[Code]](https://github.com/tulerfeng/Video-R1)      |      |      |         |
| 25.01 | Temporal Preference Optimization for Long-Form Video Understanding [[Paper]](https://arxiv.org/abs/2501.13919) |      |      |         |
|       | Tarsier2: Advancing Large Vision-Language Models from Detailed Video Description to Comprehensive Video Understanding |      |      |         |
| 25.02 | video-SALMONN-o1: Reasoning-enhanced Audio-visual Large Language Model [[Paper]](https://arxiv.org/abs/2502.11775) |      |      |         |

### Image Generation

TODO

### LLM

| Date | Project                                                      | Comment |
| ---- | ------------------------------------------------------------ | ------- |
|      | Multimodal Chain-of-Thought Reasoning in Language Models [[Code]](https://github.com/amazon-science/mm-cot) |         |



## Data
| Date | Project                                                      | Comment |
| ---- | ------------------------------------------------------------ | ------- |
|      |  |         |

