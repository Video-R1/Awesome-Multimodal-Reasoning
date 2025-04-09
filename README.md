# Awesome-Multimodal-Reasoning

**Contributions are most welcome**, if you have any suggestions or improvements, feel free to create an issue or raise a pull request.

## Contents
 - [Model](#model)
    - [Image MLLM](#image-mllm)
    - [Video MLLM](#video-mllm)
    - [Audio MLLM](#audio-mllm)
    - [Image/Video Generation](#imagevideo-generation)
    - [LLM](#llm)
 - [Benchmark](#benchmark)
 - [Data](#data)
 - [Survey Section](#survey)



## Model

### Image MLLM

| Date             | Project                                                      | SFT                                                        | RL                                                           | Task                                                         |
| ---------------- | ------------------------------------------------------------ | ---------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 25.03             | OpenVLThinker: An Early Exploration to Complex Vision-Language Reasoning via Iterative Self-Improvement [[📑Paper]]([https://arxiv.org/pdf/2503.18013v1](https://arxiv.org/pdf/2503.17352v1))[[🖥️Code]](https://github.com/yihedeng9/OpenVLThinker)  | Iterative SFT | Iterative GRPO | Various VQA| 
| 25.03            | Vision-R1: Evolving Human-Free Alignment in Large Vision-Language Models via Vision-Guided Reinforcement Learning [[📑Paper]](https://arxiv.org/pdf/2503.18013v1)[[🖥️Code]](https://github.com/jefferyZhan/Griffon/tree/master/Vision-R1) | - | GRPO | Object localization |
| 25.03            | R1-VL: Learning to Reason with Multimodal Large Language Models via Step-wise Group Relative Policy Optimization [[📑Paper]](https://arxiv.org/abs/2503.12937)[[🖥️Code]](https://github.com/jingyi0000/R1-VL) | Mulberry-260k                                              | StepGRPO with 10k data from Mulberry-260k                    | Various VQA                                                  |
| 25.03            | MetaSpatial [[🖥️Code]](https://github.com/PzySeere/MetaSpatial) | -                                                          | GRPO                                                         | 3D spatial reasoning                                         |
| 25.03            | CMMCoT: Enhancing Complex Multi-Image Comprehension via Multi-Modal Chain-of-Thought and Memory Augmentation [[📑Paper]](https://arxiv.org/pdf/2503.05255) | 260k sft                                                   | -                                                            | Multi-Image Benchmark                                        |
| 25.03            | VisualPRM: An Effective Process Reward Model for Multimodal Reasoning [[📑Paper]](https://arxiv.org/abs/2503.10291)[[model]](https://huggingface.co/OpenGVLab/VisualPRM-8B)[[data]](https://huggingface.co/datasets/OpenGVLab/VisualPRM400K)[[benchmark]](https://huggingface.co/datasets/OpenGVLab/VisualProcessBench) | -                                                          | Process Reward Model                                         | Math & MMMU                                                  |
| 25.03            | R1-Onevision: Advancing Generalized Multimodal Reasoning through Cross-Modal Formalization [[📑Paper]](https://arxiv.org/pdf/2503.10615)[[Project website]](https://yangyi-vai.notion.site/r1-onevision)[[🖥️Code]](https://github.com/Fancy-MLLM/R1-Onevision) | -                                                          | 155k R1-OneVision<br />GRPO                                  | Math                                                         |
| 25.03            | MMR1: Advancing the Frontiers of Multimodal Reasoning [[🖥️Code]](https://github.com/LengSicong/MMR1) | -                                                          | GRPO                                                         | Math                                                         |
| 25.03 (CVPR2025) | GFlowVLM: Enhancing Multi-step Reasoning in Vision-Language Models with Generative Flow Networks [[📑Paper]](https://arxiv.org/pdf/2503.06514) | -                                                          | GFlowNets                                                    | NumberLine (NL) and BlackJack (BJ)                           |
| 25.03            | VisRL: Intention-Driven Visual Perception via Reinforced Reasoning [[📑Paper]](https://arxiv.org/pdf/2503.07523)[[🖥️Code]](https://github.com/zhangquanchen/VisRL) | warm up                                                    | DPO                                                          | Various VQA                                                  |
| 25.03            | Visual-RFT: Visual Reinforcement Fine-Tuning [[📑Paper]](https://arxiv.org/abs/2503.01785)[[🖥️Code]](https://github.com/Liuziyu77/Visual-RFT) | -                                                          | GRPO                                                         | Detection, Grounding, Classification                         |
| 25.03            | LMM-R1: Empowering 3B LMMs with Strong Reasoning Abilities Through Two-Stage Rule-Based RL [[📑Paper]](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/2503.07536)[[🖥️Code]](https://github.com/TideDra/lmm-r1) | -                                                          | PPO                                                          | Math, Sokoban-Global, Football-Online                        |
| 25.03            | Boosting the Generalization and Reasoning of Vision Language Models with Curriculum Reinforcement Learning [[📑Paper]](https://arxiv.org/pdf/2503.07065) | Self-Improvement Training                                  | GRPO                                                         | Detection, Classification, Math                              |
| 25.03            | Vision-R1: Incentivizing Reasoning Capability in Multimodal Large Language Models [[📑Paper]](https://arxiv.org/abs/2503.06749)[[🖥️Code]](https://github.com/Osilly/Vision-R1) | -                                                          | GRPO                                                         | Math                                                         |
| 25.03            | Seg-Zero: Reasoning-Chain Guided Segmentation via Cognitive Reinforcement [[📑Paper]](https://arxiv.org/abs/2503.06520)[[🖥️Code]](https://github.com/dvlab-research/Seg-Zero) | -                                                          | GRPO                                                         | RefCOCO&ReasonSeg                                            |
| 25.03            | R1-Zero’s “Aha Moment” in Visual Reasoning on a 2B Non-SFT Model [[📑Paper]](https://arxiv.org/abs/2503.05132)[[🖥️Code]](https://github.com/turningpoint-ai/VisualThinker-R1-Zero) | -                                                          | GRPO                                                         | CVBench                                                      |
| 25.03            | MM-EUREKA: Exploring Visual Aha Moment with Rule-based Large-scale Reinforcement Learning [[📑Paper]](https://arxiv.org/abs/2503.07365)[[🖥️Code]](https://github.com/ModalMinds/MM-EUREKA) | -                                                          | 54.9k general science/math/chart QA<br />RLOO                | Math                                                         |
| 25.03            | Unified Reward Model for Multimodal Understanding and Generation [[📑Paper]](https://arxiv.org/abs/2503.05236)[[🖥️Code]](https://codegoat24.github.io/UnifiedReward/) | -                                                          | DPO                                                          | Various VQA & Generation                                     |
| 25.03            | EasyR1: An Efficient, Scalable, Multi-Modality RL Training Framework [[🖥️Code]](https://github.com/hiyouga/EasyR1) | -                                                          | GRPO                                                         | Geometry3K                                                   |
| 25.02            | MM-RLHF: The Next Step Forward in Multimodal LLM Alignment [[📑Paper]](https://arxiv.org/abs/2502.10391)[[🖥️Code]](https://mm-rlhf.github.io/) | -                                                          | DPO with 120k fine-grained, human-annotated preference comparison pairs. | Reward & Various VQA                                         |
| 25.02            | OmniAlign-V: Towards Enhanced Alignment of MLLMs with Human Preference [[📑Paper]](https://arxiv.org/abs/2502.18411)[[🖥️Code]](https://github.com/PhoenixZ810/OmniAlign-V) | 200k sft data                                              | DPO                                                          | Alignment & Various VQA                                      |
| 25.02            | Multimodal Open R1 [[🖥️Code]](https://github.com/EvolvingLMMs-Lab/open-r1-multimodal) | -                                                          | GRPO                                                         | Mathvista-mini, MMMU                                         |
| 25.02            | VLM-R1: A stable and generalizable R1-style Large Vision-Language Model [[🖥️Code]](https://github.com/om-ai-lab/VLM-R1/tree/main?tab=readme-ov-file) | -                                                          | GRPO                                                         | Referring Expression Comprehension                           |
| 25.02            | R1-V: Reinforcing Super Generalization Ability in Vision Language Models with Less Than $3 [[🖥️Code]](https://github.com/Deep-Agent/R1-V) | -                                                          | GRPO                                                         | Item Counting, Number Related Reasoning and Geometry Reasoning |
| 25.01            | Virgo: A Preliminary Exploration on Reproducing o1-like MLLM [[📑Paper]](https://arxiv.org/abs/2501.01904)[[🖥️Code]](https://github.com/RUCAIBox/Virgo) | 2k Text data from R1/QwQ and visual data from QvQ/SD       | -                                                            | Math & MMMU                                                  |
| 25.01            | InternLM-XComposer2.5-Reward: A Simple Yet Effective Multi-Modal Reward Model [[📑Paper]](https://arxiv.org/abs/2501.12368)[[🖥️Code]](https://github.com/InternLM/InternLM-XComposer) | -                                                          | PPO                                                          | Reward & Various VQA                                         |
| 25.01            | LlamaV-o1: Rethinking Step-By-Step Visual Reasoning in LLMs [[📑Paper]](https://arxiv.org/abs/2501.06186)[[🖥️Code]](https://github.com/mbzuai-oryx/LlamaV-o1) | LLaVA-CoT-100k & PixMo [13] subset                         | -                                                            | VRC-Bench & Various VQA                                      |
| 24.12            | Mulberry: Empowering MLLM with o1-like Reasoning and Reflection via Collective Monte Carlo Tree Search [[📑Paper]](https://arxiv.org/abs/2412.18319)[[🖥️Code]](https://github.com/HJYao00/Mulberry) | 260k reasoning and reflection sft data by Collective MCTS  | -                                                            | Various VQA                                                  |
| 24.11            | LLaVA-CoT: Let Vision Language Models Reason Step-by-Step [[📑Paper]](https://arxiv.org/abs/2411.10440)[[🖥️Code]](https://github.com/PKU-YuanGroup/LLaVA-CoT) | LLaVA-CoT-100k by GPT4-o                                   | -                                                            | Various VQA                                                  |
| 24.11            | Insight-V: Exploring Long-Chain Visual Reasoning with Multimodal Large Language Models [[📑Paper]](https://arxiv.org/abs/2411.14432)[[🖥️Code]](https://github.com/dongyh20/Insight-V) | sft for agent                                              | Iterative DPO                                                | Various VQA                                                  |
| 24.11            | Enhancing the Reasoning Ability of Multimodal Large Language Models via Mixed Preference Optimization [[📑Paper]](https://arxiv.org/abs/2411.10442) | -                                                          | MPO                                                          | Various VQA                                                  |
| 24.10            | Improve Vision Language Model Chain-of-thought Reasoning [[📑Paper]](https://arxiv.org/pdf/2410.16198)[[🖥️Code]](https://github.com/RifleZhang/LLaVA-Reasoner-DPO) | 193k CoT sft data by GPT4-o                                | DPO                                                          | Various VQA                                                  |
| 24.03            | Visual CoT: Advancing Multi-Modal Language Models with a Comprehensive Dataset and Benchmark for Chain-of-Thought Reasoning [[📑Paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/0ff38d72a2e0aa6dbe42de83a17b2223-Paper-Datasets_and_Benchmarks_Track.pdf)[[🖥️Code]](https://github.com/deepcs233/Visual-CoT) | visual chain-of-thought dataset comprising 438k data items | -                                                            | Various VQA                                                  |





### Video MLLM

| Date  | Project                                                      | SFT           | RL   | Task                |
| ----- | ------------------------------------------------------------ | ------------- | ---- | ------------------- |
| 25.03 | Open-LLaVA-Video-R1[[🖥️Code]](https://github.com/Hui-design/Open-LLaVA-Video-R1) | -             | GRPO | DVD-counting        |
| 25.03 | TimeZero: Temporal Video Grounding with Reasoning-Guided LVLM [[📑Paper]](https://arxiv.org/abs/2503.05379)[[🖥️Code]](https://github.com/www-Ye/TimeZero) | -   | GRPO | Temporal Grounding |
| 25.03 | R1-Omni: Explainable Omni-Multimodal Emotion Recognition with Reinforcement Learning [[📑Paper]](https://arxiv.org/abs/2503.05379)[[🖥️Code]](https://github.com/HumanMLLM/R1-Omni) | cold start    | GRPO | Emotion recognition |
| 25.02 | video-SALMONN-o1: Reasoning-enhanced Audio-visual Large Language Model [[📑Paper]](https://arxiv.org/abs/2502.11775) | cold start    | DPO  | various video QA    |
| 25.02 | Open-R1-Video[[🖥️Code]](https://github.com/Wang-Xiaodong1899/Open-R1-Video) | -             | GRPO | LongVideoBench      |
| 25.02 | Video-R1: Towards Super Reasoning Ability in Video Understanding [[🖥️Code]](https://github.com/tulerfeng/Video-R1) | -             | GRPO | DVD-counting        |
| 25.01 | Temporal Preference Optimization for Long-Form Video Understanding [[📑Paper]](https://arxiv.org/abs/2501.13919)[[🖥️Code]](https://ruili33.github.io/tpo_website/) | -             | DPO  | various video QA    |
| 25.01 | Tarsier2: Advancing Large Vision-Language Models from Detailed Video Description to Comprehensive Video Understanding [[📑Paper]](https://arxiv.org/abs/2501.07888)[[🖥️Code]]() | main training | DPO  | Video caption & QA  |

### Audio MLLM

| Date  | Project                                                      | SFT           | RL   | Task                |
| ----- | ------------------------------------------------------------ | ------------- | ---- | ------------------- |
| 25.03 | Reinforcement Learning Outperforms Supervised Fine-Tuning: A Case Study on Audio Question Answering [[📑Paper]](https://arxiv.org/abs/2503.11197)[[🖥️Code]](https://github.com/xiaomi-research/r1-aqa) | -             | GRPO | AudioQA        |


### Image/Video Generation

| Date  | Proj                                                         | Comment                                                    |
| ----- | ------------------------------------------------------------ | ---------------------------------------------------------- |
| 25.03 | GoT: Unleashing Reasoning Capability of Multimodal Large Language Model for Visual Generation and Editing[[📑Paper]](https://arxiv.org/pdf/2503.10639) | A reasoning-guided framework for generation and editing.   |
| 25.02 | C-Drag:Chain-of-Thought Driven Motion Controller for Video Generation[[📑Paper]](https://arxiv.org/pdf/2502.19868) | Calculate simple motion vector with LLM.                   |
| 25.01 | Can We Generate Images with CoT? Let's Verify and Reinforce Image Generation Step by Step[[📑Paper]](https://arxiv.org/pdf/2501.13926) | Potential Assessment Reward Model for AR Image Generation. |
| 25.01 | Imagine while Reasoning in Space: Multimodal Visualization-of-Thought[[📑Paper]](https://arxiv.org/pdf/2501.07542) | Visualization-of-Thought                                   |
| 25.01 | ReFocus: Visual Editing as a Chain of Thought for Structured Image Understanding[[📑Paper]](https://arxiv.org/pdf/2501.05452) | Draw something!                                            |
| 24.12 | EVLM: Self-Reflective Multimodal Reasoning for Cross-Dimensional Visual Editing[[📑Paper]](https://arxiv.org/pdf/2412.10566) | Thinking in text space with a caption model.               |



### LLM

| Date  | Project                                                      | Comment |
| ----- | ------------------------------------------------------------ | ------- |
| 25.04.09 | VAPO: Efficient and Reliable Reinforcement Learning for Advanced Reasoning Tasks[[📑Paper]](https://arxiv.org/pdf/2504.05118) |  |
| 25.03 | DAPO: An Open-Source LLM Reinforcement Learning System at Scale[[📑Paper]](https://arxiv.org/pdf/2503.14476)[[Project]](https://dapo-sia.github.io/)   | DAPO-Math-17K |
| 23.02 | Multimodal Chain-of-Thought Reasoning in Language Models [[📑Paper]](https://arxiv.org/abs/2302.00923) [[🖥️Code]](https://github.com/amazon-science/mm-cot) |         |



## Benchmark

| Date  | Project                                                      | Task                                                         |
| ----- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 25.03 | Exploring the Effect of Reinforcement Learning on Video Understanding: Insights from SEED-Bench-R1[[📑Paper]](https://arxiv.org/pdf/2503.24376) | Video understanding(perception and reasoing)                 |
| 25.03 | Does Chain-of-Thought Reasoning Help Mobile GUI Agent? An Empirical Study[[📑Paper]](https://arxiv.org/pdf/2503.16788)[[Data]](https://github.com/LlamaTouch/VLM-Reasoning-Traces) | static and dynamic mobile GUI benchmarks (ScreenSpot, AndroidControl, and AndroidWorld) |
| 25.03 | SCIVERSE: Unveiling the Knowledge Comprehension and Visual Reasoning of LMMs on Multi-modal Scientific Problems [[📑Paper]](https://arxiv.org/pdf/2503.10627) | SCIVERSE                                                     |
| 25.03 | Integrating Chain-of-Thought for Multimodal Alignment: A Study on 3D Vision-Language Learning [[📑Paper]](https://arxiv.org/pdf/2503.06232)[[Data]](https://huggingface.co/datasets/Battam/3D-CoT) | 3D-CoT                                                       |
| 25.02 | MM-IQ: Benchmarking Human-Like Abstraction and Reasoning in Multimodal Models [[📑Paper]](https://arxiv.org/pdf/2502.00698)[[🖥️Code]](https://github.com/AceCHQ/MMIQ) | MM-IQ                                                        |
| 25.02 | MM-RLHF: The Next Step Forward in Multimodal LLM Alignment [[📑Paper]](https://arxiv.org/abs/2502.10391) | MM-RLHF-RewardBench, MM-RLHF-SafetyBench                     |
| 25.02 | MME-CoT: Benchmarking Chain-of-Thought in LMMs for Reasoning Quality, Robustness, and Efficiency [[📑Paper]](https://arxiv.org/pdf/2502.09621)[[🖥️Code]](https://github.com/CaraJ7/MME-CoT) | MME-CoT                                                      |
| 25.02 | OmniAlign-V: Towards Enhanced Alignment of MLLMs with Human Preference [[📑Paper]](https://arxiv.org/abs/2502.18411)[[🖥️Code]](https://github.com/PhoenixZ810/OmniAlign-V) | MM-AlignBench                                                |
| 25.01 | LlamaV-o1: Rethinking Step-By-Step Visual Reasoning in LLMs [[📑Paper]](https://arxiv.org/abs/2501.06186)[[🖥️Code]](https://github.com/mbzuai-oryx/LlamaV-o1) | VRCBench                                                     |
| 24.11 | VLRewardBench: A Challenging Benchmark for Vision-Language Generative Reward Models [[📑Paper]](https://arxiv.org/abs/2411.17451) | VLRewardBench                                                |
| 24.05 | M3CoT: A Novel Benchmark for Multi-Domain Multi-step Multi-modal Chain-of-Thought [[📑Paper]](https://arxiv.org/html/2405.16473v1) | M3CoT                                                        |



## Data

| Date  | Project                                                      | Comment          |
| ----- | ------------------------------------------------------------ | ---------------- |
| 24.11 | VideoEspresso: A Large-Scale Chain-of-Thought Dataset for Fine-Grained  Video Reasoning via Core Frame Selection[[📑Paper]](https://arxiv.org/abs/2411.14794)[[🖥️Code]](https://github.com/hshjerry/VideoEspresso) | various video QA |

## Survey

| Date  | Project                                                      | Comment |
| ----- | ------------------------------------------------------------ | ------- |
| 25.03 | A Survey of Efficient Reasoning for Large Reasoning Models: Language, Multimodality, and Beyond[[📑Paper]](https://arxiv.org/abs/2503.21614) |  |
| 25.03 | Aligning Multimodal LLM with Human Preference: A Survey[[📑Paper]](https://arxiv.org/abs/2503.14504) |         |
