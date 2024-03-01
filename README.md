---
datasets:
- allenai/objaverse
tags:
- 3d
extra_gated_fields:
  Name: text
  Email: text
  Country: text
  Organization or Affiliation: text
  I ALLOW Stability AI to email me about new model releases: checkbox
license: mit
pipeline_tag: image-to-3d
---
# TripoSR

## Model Description

TripoSR is a fast and feed-forward 3D generative model developed in partnership with Tripo AI inspired by the recent work of [LRM: Large Reconstruction Model For Single Image to 3D](https://arxiv.org/abs/2311.04400).

This new image-to-3D model leverages cutting-edge AI advancements to set new standards in 3D model generation. Designed to cater to the growing demands of entertaining, gaming, industrial design, and architecture professionals, TripoSR enriches the conversion process with detail and precision while providing efficient and responsive outputs for visualizing 3D objects.

![row01](figures/output_examples.mov)

## Usage

For usage instructions, please refer to our [TripoSR GitHub repository](https://github.com/VAST-AI-Research/TripoSR).

## Model Details

### Model Description

We closely follow [LRM](https://arxiv.org/abs/2311.04400) network architecture for the model design, where TripoSR incorporates a series of technical advancements over the LRM model in terms of both data curation as well as model and training improvements. For more technical details and evaluations, please refer to [the tech report on our model](link).

* **Developed by**: [Stability AI](https://stability.ai/), [Tripo AI](https://tripo3d.ai/)
* **Model type**: Feed-forward model
* **License**: MIT
* **Hardware**: `TripoSR` was trained on the Stability AI cluster on 22 nodes with 8 A100 40GBs GPUs for 5 days.

### Model Sources

* **Repository**: https://github.com/VAST-AI-Research/TripoSR
* **Tech report**: *link*

### Training Dataset

We use renders from the [Objaverse](https://objaverse.allenai.org/objaverse-1.0) dataset, utilizing our enhanced rendering method that more closely replicate the distribution of images found in the real world, significantly improving our model’s ability to generalize. We selected a carefully curated subset of the Objaverse dataset for the training data, which is available under the CC-BY license. 


### Misuse, Malicious Use, and Out-of-Scope Use

The model should not be used to intentionally create or disseminate 3D models that people would foreseeably find disturbing, distressing, or offensive; or content that propagates historical or current stereotypes.