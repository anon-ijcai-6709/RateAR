# RateAR
This repository introduces **RateAR**, a dataset of 321 AR images and 112 AR videos collected from various platforms and scenarios.

# Dataset
The full RateAR dataset will be available for download by August 2026, if not sooner. The dataset follows the hierarchical file structure shown below:
```
dataset
└───rateAR_images
│   └───RateAR_Images_MOS_Metadata.csv
│   └───AVP
│   │   └───AVP_can
│   │   │   └───AVP_can_1_ar.png
│   │   │   ...
│   │   ...
│   └───andriod
│   ...
└───rateAR_videos
│   └───RateAR_Videos_MOS_Metadata.csv
│   └───livingroom
│   │   └───livingroom_tire_1_1_1.mp4
│   │   ...
│   └───dorm
│   ...
```

_Dataset Composition:_ The RateAR dataset comprises 321 AR images and 112 AR videos. Sample curation aimed to diversify the observed visual quality among influential user immersion properties. Figure 1 presents representative examples from RateAR, illustrating a range of quality levels across three key visual factors: placement plausibility, size appropriateness, and shadow realism.

_AR Platforms:_ AR samples are sourced from a range of devices and scenarios. 321 AR images are collected from **DiverseAR+** \[Duan *et al.*, 2025\], selected for their varying rendering qualities in virtual content placement, shadow, and size. All RateAR image instances were captured using Android smartphones (250), Apple Vision Pro (40), and Microsoft HoloLens 2 (31). A diverse collection of environments are featured, including bedrooms, kitchens, living rooms, medical offices, reading rooms, research labs, and study rooms. The 112 AR videos were captured by us to represent a similar distribution of quality feature variations, showcasing settings such as basements, bedrooms, living rooms, and research labs. All RateAR videos are recorded using a Meta Quest 3 head mounted display.

_Context-Dependent Scenarios:_ Alongside common settings such as bedrooms and kitchens, where assessing visual factors primarily relies on general, publicly shared knowledge, 
RateAR also includes scenes that require context-dependent reasoning for evaluation. For example, medical settings feature virtual organ models placed in anatomically accurate locations on human subjects or 3D-printed models (e.g., a skull). In these scenarios, the placement plausibility and size appropriateness of virtual content is most critical, while elements like shadow realism are less relevant for perceived quality. Additionally, we include scenarios that capture dynamic user interactions, such as a hand shown bouncing a virtual basketball. As a result, some examples with observed floating AR content may be contextually appropriate, therefore receiving a high placement plausibility score.

_Human Subjective Quality Score Labeling:_ Visual quality scores for three target features (placement plausibility, shadow realism, and size appropriateness) were rated by four AR experts. A 5-point discrete scale was employed for annotating. An assignment of 1 signifies *poor* rendered feature quality, while a score of 5 indicates *good* or exceptional visual appearance. All annotators assigned quality labels for each AR content factor, per sample, resulting in 5,196 annotations. The mean opinion scores (MOSs) are used as final ratings in our evaluations. RateAR samples were labeled using a Python notebook GUI interface.

<p align="center"><img width="600" alt="Representative cropped examples from the RateAR dataset illustrating various quality levels across three visual features of interest." src="https://github.com/anon-ijcai-6709/RateAR/blob/main/RateAR_samples.png"></p>
<p align="center">Figure 1. Representative cropped examples from the RateAR dataset illustrating various quality levels across three visual features of interest: (1) Placement plausibility: virtual wooden desk rendered a few feet above the ground (poor), a few inches above the ground (fair), and level with the ground (good); (2) Size appropriateness: digital car modeled next to a real-world vehicle that appears far too small (poor), slightly too small (fair), and realistically sized (good); and (3) Shadow realism: AR noodle bowl shown with virtual shadow facing the opposite direction (poor), shadow slightly misaligned with real-world object shadows (fair), and shadow aligned with natural light source and real shadows (good).</p> 
