# End-to-End Differentiable Visible-SWIR Image Fusion for Robust Perception in Adverse Weather

<div align="center">

[![Conference](https://img.shields.io/badge/ICARCV_2026-Accepted-success.svg?style=flat-square)](https://www.carvs-icarcv.org/)
[![Paper Status](https://img.shields.io/badge/Paper-Accepted-blue.svg?style=flat-square)]()
<!-- [![Framework](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)](https://pytorch.org/) -->
[![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg?style=flat-square)](https://www.gnu.org/licenses/lgpl-3.0)

**Official repository for the paper accepted at the 19th International Conference on Control, Automation, Robotics and Vision (ICARCV 2026).**

[**Alexandre Riffard**](https://github.com/AlexandreRiffard)<sup>1</sup> · [**Mathieu Labussiere**](https://github.com/MathieuLabussiere)<sup>1</sup> · [**Pierre Duthon**](https://github.com/Pierreduthon)<sup>2</sup> · [**Romuald Aufrere**](https://github.com/RomualdAufrere)<sup>1</sup>

<sup>1</sup> Université Clermont Auvergne, Clermont Auvergne INP, CNRS, Institut Pascal, Clermont-Ferrand, France  
<sup>2</sup> Cerema, Research Team "Intelligent Transport Systems", Clermont-Ferrand, France  
✉️ Contact: `{alexandre.riffard, mathieu.labussiere, romuald.aufrere}@uca.fr`, `pierre.duthon@cerema.fr`

</div>

---

## 📢 Repository Status: *Coming Soon*

> [!NOTE]
> This repository is a placeholder accompanying our ICARCV 2026 paper.  
> The full source code, pre-trained models, and instructions will be made publicly available upon official publication of the paper.

---

## 📖 Abstract

Reliable perception in adverse weather, such as dense fog, heavy rain, or severe glare, remains a critical challenge for Autonomous Vehicles (AV).  
While visible (VIS) cameras degrade rapidly in these conditions, Short-Wave Infrared (SWIR) sensors offer enhanced atmospheric penetration and structural retention.  
However, fusing VIS and SWIR is hampered by sensor noise, modality misalignment, and the lack of pixel-perfect ground truth.  
In this paper, we propose Diff-VISWIR, a prior-guided, end-to-end differentiable fusion architecture.  
Moving away from purely data-driven architectures, our method unrolls a physical Laplacian pyramid into a learnable network.  
It introduces a modality-specific saliency extractor and a soft-veto mechanism that dynamically suppresses the VIS contribution when robust SWIR structures are detected.  
The architecture is explicitly constrained by physical and colourimetric bounds, and optimised via a semantic-aware multi-objective loss that includes supervision from a downstream object detector.  
Experimental results demonstrate that Diff-VISWIR achieves robust zero-shot domain generalisation.  
On a severely degraded dataset, it delivers top-tier downstream detection performance, achieving high precision while mitigating the formation of false-positive contours under adverse conditions.  
Furthermore, our framework operates at 33-37 frames per second on high-definition automotive inputs, satisfying real-time deployment constraints.

---

## 📝 Citation

If you find this work useful in your research, please cite our paper:

```bibtex
@inproceedings{riffard2026diffviswir,
  title     = {End-to-End Differentiable Visible-SWIR Image Fusion for Robust Perception in Adverse Weather},
  author    = {Riffard, Alexandre and Labussiere, Mathieu and Duthon, Pierre and Aufrere, Romuald},
  booktitle = {18th International Conference on Control, Automation, Robotics and Vision (ICARCV)},
  year      = {2026},
  address   = {Singapore},
  publisher = {IEEE}
}
```

---

## 🤝 Acknowledgments

This work was supported by the **International Research Center "Innovation Transportation and Production Systems"** of the **I-SITE CAP 20-25**.  
We thank the **Institut Pascal (Université Clermont Auvergne, Clermont Auvergne INP, CNRS)** and **Cerema (Team Intelligent Transport Systems)** for their support.

---

## 📄 License

This project is licensed under the GNU Lesser General Public License v3.0 (LGPL-3.0) - see the [LICENSE](LICENSE) file for details.
