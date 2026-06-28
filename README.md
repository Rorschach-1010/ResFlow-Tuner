# 🚀 ResFlow-Tuner: Tuning Real-World Image Restoration at Inference: A Test-Time Scaling Paradigm for Flow Matching Models

[![Paper](https://img.shields.io/badge/arXiv-Paper-<COLOR>.svg)](https://arxiv.org/abs/2603.22027)
[![ECCV 2026](https://img.shields.io/badge/ECCV-2026-blue.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

> **Tuning Real-World Image Restoration at Inference: A Test-Time Scaling Paradigm for Flow Matching Models** <br>
> Purui Bai, Huaibo Huang, Junxian Duan, Pin Wang, et al.<br>
> Accepted by **ECCV 2026**

This is the official PyTorch implementation and model weights for the ECCV 2026 paper **ResFlow-Tuner**. 

ResFlow-Tuner introduces a pioneering **Test-Time Scaling (TTS)** paradigm for flow-based Image Restoration (IR). By formulating a task-specific zero-drift SDE discretization and introducing the **Unified Multi-Modal Fusion (UMMF)** mechanism, we achieve state-of-the-art structural recovery and fidelity with extreme parameter efficiency.

> **🚧 🚧 TODO / Coming Soon 🚧 🚧** <br>
> **The source code, pre-trained weights, and full evaluation scripts are currently under internal review and being cleaned up. We will release them here soon. Stay tuned!**

---

## 📢 News
* **[TODO]** 🔥 The official PyTorch code and pre-trained weights will be released soon!
* **[2026-06]** 🎉 Our paper has been accepted by **ECCV 2026**! 

---

## 🌟 Key Features

* **Zero-Drift SDE for TTS**: Overcomes the deterministic ODE limitation in Flow models. By setting the drift term to zero, it allows test-time search to optimize strictly along local trajectories for exact structural recovery without uncontrolled semantic variations.
* **Unified Multi-Modal Fusion (UMMF)**: A highly efficient tri-modal sequence fusion $([z_{t}; C_{img}; C_{txt}])$ that explicitly separates structural and semantic guidance.
* **Compute-Aware Flexibility**: Establishes a clear cost-performance Pareto frontier. Use the base model for ultra-fast inference, or scale up test-time compute (adjusting intervention rounds $K$ and candidates $N$) for maximum fidelity.

---

## 👁️ Visual Results

*(TODO: Add a grid of visual comparisons here. Show your Best Results, especially the Old Photos restoration and comparisons with SUPIR / DiT4SR)*

<details>
<summary>Click to see more visual comparisons</summary>
<p align="center">
  <!-- TODO: Update image path when assets are uploaded -->
  <img src="assets/comparison1.png" width="800">
</p>
</details>

---

## 🛠️ Installation (TODO)

*Instructions will be updated upon code release.*

```bash
# [Preview]
git clone [https://github.com/your-username/ResFlow-Tuner.git](https://github.com/your-username/ResFlow-Tuner.git)
cd ResFlow-Tuner
conda create -n resflow python=3.10
conda activate resflow
pip install -r requirements.txt
