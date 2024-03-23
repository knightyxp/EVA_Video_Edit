# EVA

**[EVA: Zero-shot Accurate Attributes and Multi-Object Video Editing](https://arxiv.org/)**
<br/>
[Xiangpeng Yang](https://github.com/knightyxp),
[Linchao Zhu](https://ffmpbgrnn.github.io/),
[Hehe Fan](https://hehefan.github.io/),
[Yi Yang](https://scholar.google.com/citations?user=RMSuNFwAAAAJ&hl=en),
<br/>

[![arXiv](https://img.shields.io/badge/arXiv-2312.02087-b31b1b.svg)](https://arxiv.org/)
[![Project Page](https://img.shields.io/badge/Project-Website-orange)](https://knightyxp.github.io/EVA/)

## 📣 EVA Intro Video

https://github.com/knightyxp/EVA_Video_Edit/assets/48432506/fca0bf8a-3e31-4696-82a2-6154e57967e5

**EVA** can achieves **accurate multi-attribute editing**  editing for both single and **multi-object** scenarios in human-centric complex motion. **Without any training** by leveraging pre-trained **text-image** SD models.  

>Current diffusion-based video editing primarily focuses on local editing (object/background editing) or global style editing by utilizing various dense correspondences. However, these methods often fail to accurately edit the foreground and background simultaneously while preserving the original layout. We find that the crux of the issue stems from the imprecise distribution of attention weights across designated regions, including inaccurate text-to-attribute control and attention leakage.
To tackle this issue, we introduce EVA, a zero-shot and multi-attribute video editing framework tailored for human-centric videos with complex motions. We incorporate a Spatial-Temporal Layout-Guided Attention mechanism that leverages the intrinsic positive and negative correspondences of cross-frame diffusion features.To avoid attention leakage, we utilize these correspondences to boost the attention scores of tokens within the same attribute across all video frames while limiting interactions between tokens of different attributes in the self-attention layer. For precise text-to-attribute manipulation, we use discrete text embeddings focused on specific layout areas within the cross-attention layer. Benefiting from the precise attention weight distribution, EVA can be easily generalized to multi-object editing scenarios and achieves accurate identity mapping. Extensive experiments demonstrate EVA achieves state-of-the-art results in real-world scenarios.

For more see the [project webpage](https://knightyxp.github.io/EVA/).

## Acknowledgements

This codebase builds on [diffusers](https://github.com/huggingface/diffusers). Besides, we acknowledge following amazing open-sourcing projects:

- FazteZero (https://github.com/ChenyangQiQi/FateZero).


- controlvideo (https://github.com/thu-ml/controlvideo).


## 📌 Citation

```bibtex

@article{yang2024eva,
  title={EVA: Zero-shot Accurate Attributes and Multi-Object Video Editing},
  author={Xiangpeng Yang, Linchao Zhu, Hehe Fan, Yi Yang},
  journal={arXiv preprint arXiv:},
  year={2024}
}

```