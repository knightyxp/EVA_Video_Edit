# EVA: Zero-shot Accurate Attributes and Multi-Object Video Editing

**[EVA: Zero-shot Accurate Attributes and Multi-Object Video Editing](https://arxiv.org/abs/2403.16111)**
<br/>
[Xiangpeng Yang](https://github.com/knightyxp),
[Linchao Zhu](https://ffmpbgrnn.github.io/),
[Hehe Fan](https://hehefan.github.io/),
[Yi Yang](https://scholar.google.com/citations?user=RMSuNFwAAAAJ&hl=en),
<br/>

[![arXiv](https://img.shields.io/badge/arXiv-2312.02087-b31b1b.svg)](https://arxiv.org/abs/2403.16111)
[![Project Page](https://img.shields.io/badge/Project-Website-orange)](https://knightyxp.github.io/EVA/)

![teaser](assets/teaser.gif)
(Note that the videos on GitHub are heavily compressed. The full videos are available on the project webpage.)

📚 TL; DR: **EVA**  is based on **T2I model** (StableDiffusion 1.5), designed for accurate **multi-attribute** editing in **single/multi-object** scenarios **without any training**.

## 📣 EVA Intro Video

https://github.com/knightyxp/EVA_Video_Edit/assets/48432506/c474474b-904f-4896-8ee5-3acf3b187df2


<details><summary>Click for the full abstract</summary>

>Current diffusion-based video editing primarily focuses on local editing (object/background editing) or global style editing by utilizing various dense correspondences. However, these methods often fail to accurately edit the foreground and background simultaneously while preserving the original layout. We find that the crux of the issue stems from the imprecise distribution of attention weights across designated regions, including inaccurate text-to-attribute control and attention leakage.
To tackle this issue, we introduce EVA, a zero-shot and multi-attribute video editing framework tailored for human-centric videos with complex motions. We incorporate a Spatial-Temporal Layout-Guided Attention mechanism that leverages the intrinsic positive and negative correspondences of cross-frame diffusion features.To avoid attention leakage, we utilize these correspondences to boost the attention scores of tokens within the same attribute across all video frames while limiting interactions between tokens of different attributes in the self-attention layer. For precise text-to-attribute manipulation, we use discrete text embeddings focused on specific layout areas within the cross-attention layer. Benefiting from the precise attention weight distribution, EVA can be easily generalized to multi-object editing scenarios and achieves accurate identity mapping. Extensive experiments demonstrate EVA achieves state-of-the-art results in real-world scenarios.
</details>


## 🔥 Project page
For more editing results, plz see [project webpage](https://knightyxp.github.io/EVA/).


<!-- ## ⚡️ Showcases
<table class="center">
  <tr>
    <td colspan="1">single attribute editing →   multi attribute editing</td>
    <td colspan="1"> multi object editing →  swap identity</td>
  </tr>
  <tr>
  <td>
    <img src=assets/tennis.gif width="700">
  </td>

  <td>
    <img src=assets/running_two_man.gif width="700">
  </td>

  </tr>


</table> -->



## Acknowledgements

This codebase builds on [diffusers](https://github.com/huggingface/diffusers). Besides, we acknowledge following amazing open-sourcing projects:

- FazteZero (https://github.com/ChenyangQiQi/FateZero).


- controlvideo (https://github.com/thu-ml/controlvideo).


## 📌 Citation
If you find this paper useful, please consider staring 🌟 this repo and citing 📑 our paper:
```bibtex

@misc{yang2024eva,
      title={EVA: Zero-shot Accurate Attributes and Multi-Object Video Editing}, 
      author={Xiangpeng Yang and Linchao Zhu and Hehe Fan and Yi Yang},
      year={2024},
      eprint={2403.16111},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}

```