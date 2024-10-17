## [ECCV 2024] GMT: Enhancing Generalizable Neural Rendering via Geometry-Driven Multi-Reference Texture Transfer <br><sub>Official PyTorch Implementation of GMT. </sub>

[Paper](https://arxiv.org/abs/2410.00672)

## Introduction

Novel view synthesis (NVS) aims to generate images at arbitrary viewpoints using multi-view images, and recent insights from neural radiance fields (NeRF) have contributed to remarkable improvements. Recently, studies on generalizable NeRF (G-NeRF) have addressed the challenge of per-scene optimization in NeRFs. The construction of radiance fields on-the-fly in G-NeRF simplifies the NVS process, making it well-suited for real-world applications. Meanwhile, G-NeRF still struggles in representing fine details for a specific scene due to the absence of perscene optimization, even with texture-rich multi-view source inputs. As a remedy, we propose a Geometry-driven Multi reference Texture transfer network (GMT) available as a plug-and-play module designed for G-NeRF. Specifically, we propose ray-imposed deformable convolution (RayDCN), which aligns input and reference features reflecting scene geometry. Additionally, the proposed texture preserving transformer (TPFormer) aggregates multi-view source features while preserving texture information. Consequently, our module enables direct interaction between adjacent pixels during the image enhancement process, which is deficient in G-NeRF models with an independent rendering process per pixel. This addresses constraints that hinder the ability to capture highfrequency details. Experiments show that our plug-and-play module consistently improves G-NeRF models on various benchmark datasets.

### Framework
![image](Images/framework.png)

# Citation

If you find this project helpful in your research, welcome to cite the paper.

```
@article{yoon2024gmt,
  title={GMT: Enhancing Generalizable Neural Rendering via Geometry-Driven Multi-Reference Texture Transfer},
  author={Yoon, Youngho and Jang, Hyun-Kurl and Yoon, Kuk-Jin},
  journal={arXiv preprint arXiv:2410.00672},
  year={2024}
}
```

# Contact

Please contact Youngho Yoon if there is any question (dudgh1732@kaist.ac.kr).
