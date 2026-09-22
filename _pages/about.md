---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome to my personal page! 

I am currently a second-year Joint Master's student at the Southern University of Science and Technology and the Shenzhen Institutes of Advanced Technology, CAS, advised by Prof. Xinyu Wu and Prof. Zhengkun Yi. In addition, I serve as a Research Assistant at The Chinese University of Hong Kong under the supervision of Prof. Li Zhang.

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
  * **Date:** Sept. 2020 - July 2024 (Guangzhou, China), GPA: 3.63 / 4.0
  * **Advisor:** Prof. Yong Zhong
  * **Awards:** Outstanding Bachelor's Thesis (Top 5%), National Scholarship (2022-2023), University Outstanding Student Club Leader
  
## Research Experience
<div style="border: 1.5px solid #d1d5db; padding: 20px; border-radius: 10px; margin-bottom: 25px;" markdown="1">
  
<h3 style="margin-top: 0;">Bio-inspired Event-frame Dual-modal Tactile Sensing</h3>

*   **Overview:** 
    Existing vision-based tactile sensors typically rely on a single modality, either event-based or frame-based. We designed a innovative event-frame dual-modal robotic tactile sensor with a DAVIS346 camera, which can synchronously capture microsecond-resolution dynamic event streams and rich static grayscale frames, replicating the fast-slow dual-pathway perception mechanism of human fingers. This approach significantly enhances robotic tactile perception and enables the system to excel at challenging material discrimination tasks.

<div align="center">
  <!-- 00.jpg -->
  <img src="/images/00.jpg" width="90%" style="margin-top: 10px;">
  <p style="font-size: 0.9em; color: gray;"><em>Figure 1: Event-frame dual modal robotic tactile sensor.</em></p>
</div>

*   **Multimodal Network:** 
    We developed a three stage fusion method to effectively integrate the visual and dynamic signals. The pipeline encompasses frame synchronized event accumulation, independent training through a shared Transformer architecture, and dynamic decision level fusion to maximize the complementary strengths of both modalities.

<div align="center">
  <!-- 1.jpg -->
  <img src="/images/1.jpg" width="90%" style="margin-top: 10px; margin-bottom: 10px;">
  <p style="font-size: 0.9em; color: gray;"><em>Figure 2: The proposed multimodal fusion network architecture.</em></p>
</div>

*   **Experiments & Results:** 
    We evaluated the sensor and network on two highly challenging tactile tasks. For texture discrimination involving lateral sliding on ten diverse fabrics, the dual modal approach achieved 91.67% accuracy, which outperformed the best single modality by 13.34%. For stiffness classification involving vertical pressing on ten polyurethane foams, the system achieved 98.92% accuracy, exceeding the best single modality by 6.47%. These results demonstrate that combining event and frame modalities significantly enhances the capability to distinguish subtle material differences.

<div align="center">
  <!-- 2.jpg -->
  <img src="/images/2.jpg" width="90%" style="margin-top: 10px; margin-bottom: 10px;">
  <p style="font-size: 0.9em; color: gray;"><em>Figure 3: Experiment on texture and stiffness classification tasks.</em></p>
</div>
    
*   **Key Innovations:**
    *   **Dual-modal Sensor:** Developed a novel event frame dual modal tactile sensor that authentically replicates the fast slow dual pathway perception mechanism of the human tactile system.
    *   **Fusion Network:** Proposed a three stage multimodal fusion method featuring frame synchronized event accumulation, a shared Transformer architecture, and dynamic decision level fusion.
    *   **Experimental Performance:** Evaluated the system on highly challenging texture and stiffness classification tasks, significantly outperforming the best single modality by up to 13.34%.

</div>

<div style="border: 1.5px solid #d1d5db; padding: 20px; border-radius: 10px; margin-bottom: 25px;" markdown="1">
  
<h3 style="margin-top: 0;">Collaborative Snap-Fit Assembly via Fingertip Iontronic Film and Wrist Six-Axis Force Sensing</h3>

*   **Overview:** 
    During delicate assembly tasks, humans fundamentally rely on the coordination of multiple tactile perception systems. In wrist-fingertip synergy, the wrist detects global multi-directional force disturbances, whereas the fingertips are acutely sensitive to subtle variations from direct contact. To emulate this biological mechanism, we integrated a wrist-mounted six-axis force sensor with a custom-fabricated iontronic film attached to the robotic gripper. We successfully validated the critical complementarity of wrist force and fingertip iontronic tactile feedback through the precision snap-fit assembly of Type-A and Type-C connectors.
    
<div align="center">
  <!-- a.png -->
  <img src="/images/a.png" width="90%" style="margin-top: 10px; margin-bottom: 10px;">
  <p style="font-size: 0.9em; color: gray;"><em>Figure 1: The fingertip iontronic film and wrist six-axis force sensor.</em></p>
</div>


*   **Complementarity Analysis:** 
    In snap-fit assembly, a successful insertion occurs when the plug is fully inserted, colliding with the socket bottom to connect. Failures are primarily categorized into two types: Type 1 (partial insertion without bottoming out) and Type 2 (severe misalignment causing collisions outside the socket). For Type 1 failures, the lack of collision allows the wrist six-axis force sensor alone to achieve an 85.14% accuracy in our Type-C experiments. However, both Type 2 failures and successful insertions generate significant force peaks due to collisions. This macro-level mechanical similarity causes the wrist force sensor to struggle, yielding only a 68.7% accuracy when classifying Success vs. Type 2 failures.

<div align="center">
  <!-- 1.mp4 -->
  <video width="100%" controls autoplay loop muted style="margin-top: 10px; margin-bottom: 10px;">
    <source src="/images/1.mp4" type="video/mp4">
  </video>
  <p style="font-size: 0.9em; color: gray;"><em>Video 2: Comparison of Success, Type 1 failure (partial insertion), and Type 2 failure (misalignment).</em></p>
</div>

*   **Multimodal Fusion Performance:** 
    This ambiguity highlights the critical complementarity of fingertip tactile sensing. While wrist force struggles with collision similarities, the fingertip iontronic film is exquisitely sensitive to subtle vibrations, effectively capturing the crucial transient "click" features of the snap-fit engagement—a mechanism closely mirroring the human tactile system. By integrating fingertip tactile feedback, the classification accuracy for Success vs. Type 2 failures significantly improves to 78.76% (a 10.06% gain). Furthermore, in a generalized binary classification task (Success vs. Any Failure), our dual-modal fusion framework achieves an impressive overall accuracy of 90.4%.



</div>
