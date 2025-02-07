---
title: "HouseCrafter: Lifting Floorplans to 3D Scenes with 2D Diffusion Model"
collection: publications
permalink: housecrafter
venue: 'Arxiv'
paperurl: 'https://arxiv.org/abs/2406.20077'
projecturl: 'https://neu-vi.github.io/houseCrafter/'
# codeurl: 'https://arxiv.org/abs/2009.12111'
authors: '<b>Hieu T. Nguyen*</b>, Yiwen Chen*, Vikram Voleti, Varun Jampani, Huaizu Jiang'
equal: "true"
teaser: "housecrafter_paper.gif"
---

We introduce HouseCrafter, a novel approach that can lift a floorplan into a complete large 3D indoor scene (e.g., a house). Our key insight is to adapt a 2D diffusion model, which is trained on web-scale images, to generate consistent multi-view color (RGB) and depth (D) images across different locations of the scene. Specifically, the RGB-D images are generated autoregressively in a batch-wise manner along sampled locations based on the floorplan, where previously generated images are used as condition to the diffusion model to produce images at nearby locations. The global floorplan and attention design in the diffusion model ensures the consistency of the generated images, from which a 3D scene can be reconstructed. Through extensive evaluation on the 3D-Front dataset, we demonstrate that HouseCraft can generate high-quality house-scale 3D scenes. Ablation studies also validate the effectiveness of different design choices. We will release our code and model weights.