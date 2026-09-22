---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome to my personal page! 

I am currently a second-year Joint Master's student at the Southern University of Science and Technology (SUSTech) and the Shenzhen Institutes of Advanced Technology (SIAT), CAS, advised by Prof. Xinyu Wu (IEEE Fellow) and Prof. Zhengkun Yi. In addition, I serve as a Research Assistant at The Chinese University of Hong Kong (CUHK) under the supervision of Prof. Li Zhang (IEEE Fellow).

🔥 **I am actively seeking PhD opportunities starting in Fall 2027. My research primarily focuses on robotic tactile perception, multimodal learning, soft robotics, and dexterous hands**.

📍 **Upcoming:** I will be presenting our work on bio-inspired event-frame dual-modal tactile sensors at **IROS 2026**. Catch my presentation at the *Focused - Reinventing the Tactile Sensor* session on Wednesday, Sept. 30 (09:00 - 09:44) in Room 326. I would love to connect and chat if you are also attending!

## Education & Experience

* **Master's Degree, Joint Program**
  * *Southern University of Science and Technology (SUSTech) & Shenzhen Institutes of Advanced Technology (SIAT), CAS*
  * **Date:** Sept. 2024 - Expected June 2027 (Shenzhen, China)
  * **Advisors:** Prof. Xinyu Wu (IEEE Fellow) & Prof. Zhengkun Yi
  * **Research Area:** Tactile sensing technology and multimodal fusion

* **Research Assistant**
  * *The Chinese University of Hong Kong (CUHK)*
  * **Date:** May 2026 - Present (Hong Kong, China)
  * **Advisor:** Prof. Li Zhang (IEEE Fellow)
  * **Research Area:** Wrist-fingertip collaborative tactile perception; Iontronic tactile sensing

* **Bachelor's Degree, Robotics Engineering (English-Taught)**
  * *South China University of Technology (SCUT)*
  * **Date:** Sept. 2020 - July 2024 (Guangzhou, China), **GPA:** 3.63 / 4.0
  * **Advisor:** Prof. Yong Zhong
  * **Awards:** Outstanding Bachelor's Thesis (Top 5%), National Scholarship (2022-2023), University Outstanding Student Club Leader
  
## Research Experience

*   **Bio-inspired Event-frame Dual-modal Tactile Sensing**
    *   **Overview:** Existing vision-based tactile sensors typically rely on a single modality, either event-based or frame-based. We designed a innovative event-frame dual-modal robotic tactile sensor with a DAVIS346 camera, which can synchronously capture microsecond-resolution dynamic event streams and rich static grayscale frames, replicating the fast-slow dual-pathway perception mechanism of human fingers. This approach significantly enhances robotic tactile perception and enables the system to excel at challenging material discrimination tasks.

    <div align="center">
      <img src="/images/00.jpg" width="50%" style="margin-top: 10px;">
      <p style="font-size: 0.9em; color: gray;"><em>Figure 1: Event-frame dual modal robotic tactile sensor.</em></p>
    </div>

*   **Multimodal Network:** We developed a three stage fusion method to effectively integrate the visual and dynamic signals. The pipeline encompasses frame synchronized event accumulation, independent training through a shared Transformer architecture, and dynamic decision level fusion to maximize the complementary strengths of both modalities.

    <div align="center">
      <img src="/images/1.jpg" width="80%" style="margin-top: 10px; margin-bottom: 10px;">
      <p style="font-size: 0.9em; color: gray;"><em>Figure 2: The proposed multimodal fusion network architecture.</em></p>
    </div>
    
*   **Key Innovations:** Developed a decision-level fusion framework featuring a shared Transformer architecture and dynamic modality-preference strategies. This methodology effectively leverages complementary static and dynamic tactile features, achieving 91.67% accuracy in 10-class fabric texture discrimination and 98.92% in polyurethane foam stiffness classification.

*   **Force-Based State Classification Networks for Robotic Assembly**
    *   Refined a polarity-aware mathematical formulation to precisely extract the minimal snap-fit engagement sequence from continuous, extended force-time traces.
    *   Implemented an automated self-labeling and sliding-window sampling pipeline that successfully expanded the original force dataset by approximately 270 times.
    *   Proposed SF-Net, a deep learning architecture integrating a residual bidirectional LSTM (R-LSTM) backbone to handle long temporal dependencies and a focal loss function to mitigate severe class imbalance. 
    *   Achieved a 96.40% classification accuracy on a public snap-fit benchmark, outperforming vanilla RNN, LSTM, and residual-RNN baselines.
