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

  
## Research Experience
<div style="border: 1.5px solid #d1d5db; padding: 20px; border-radius: 10px; margin-bottom: 25px;" markdown="1">
  
<h3 style="margin-top: 0;">Bio-inspired Event-frame Dual-modal Tactile Sensing</h3>

*   **Overview:** 
    Existing vision-based tactile sensors typically rely on a single modality, either event-based or frame-based. We designed a innovative event-frame dual-modal robotic tactile sensor with a DAVIS346 camera, which can synchronously capture microsecond-resolution dynamic event streams and rich static grayscale frames, replicating the fast-slow dual-pathway perception mechanism of human fingers. This approach significantly enhances robotic tactile perception and enables the system to excel at challenging material discrimination tasks.

<div align="center">
  <!-- 00.jpg -->
  <img src="/images/00.jpg" width="90%" style="border-radius: 10px;margin-top: 10px;">
  <p style="font-size: 0.9em; color: gray;"><em>Figure 1: Event-frame dual modal robotic tactile sensor.(IROS 2026)</em></p>
</div>

*   **Multimodal Network:** 
    We developed a three stage fusion method to effectively integrate the visual and dynamic signals. The pipeline encompasses frame synchronized event accumulation, independent training through a shared Transformer architecture, and dynamic decision level fusion to maximize the complementary strengths of both modalities.

<div align="center">
  <!-- 1.jpg -->
  <img src="/images/1.jpg" width="90%" style="margin-top: 10px; margin-bottom: 10px;">
  <p style="font-size: 0.9em; color: gray;"><em>Figure 2: The proposed multimodal fusion network architecture.(IROS 2026)</em></p>
</div>

*   **Experiments & Results:** 
    We evaluated the sensor and network on two highly challenging tactile tasks. For texture discrimination involving lateral sliding on ten diverse fabrics, the dual modal approach achieved 91.67% accuracy, which outperformed the best single modality by 13.34%. For stiffness classification involving vertical pressing on ten polyurethane foams, the system achieved 98.92% accuracy, exceeding the best single modality by 6.47%. These results demonstrate that combining event and frame modalities significantly enhances the capability to distinguish subtle material differences.

<div align="center">
  <!-- 2.jpg -->
  <img src="/images/2.jpg" width="90%" style="margin-top: 10px; margin-bottom: 10px;">
  <p style="font-size: 0.9em; color: gray;"><em>Figure 3: Experiment on texture and stiffness classification tasks.(IROS 2026)</em></p>
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


*   **Snap-fit Experiment:** 
    In snap-fit assembly, a successful insertion occurs when the plug is fully inserted and collides with the socket bottom to establish a connection. Failures are primarily categorized into two distinct types. Type 1 represents a partial insertion without bottoming out, while Type 2 involves severe misalignment that causes collisions outside the socket. For Type 1 failures, the lack of collision allows the wrist six-axis force sensor alone to achieve an 85.14% accuracy in our Type-C experiments. However, both Type 2 failures and successful insertions generate significant force peaks due to collisions. This macro-level mechanical similarity causes the wrist force sensor to struggle, yielding only a 68.7% accuracy when classifying success against Type 2 failures.

<div align="center">
  <!-- 1.mp4 -->
  <video width="90%" controls autoplay loop muted style="border-radius: 10px;margin-top: 10px; margin-bottom: 10px;">
    <source src="/images/1.mp4" type="video/mp4">
  </video>
  <p style="font-size: 0.9em; color: gray;"><em>Video 1: Comparison of Success, Type 1 failure, and Type 2 failure.</em></p>
</div>

*   **Multimodal Fusion Performance:** 
    This ambiguity highlights the critical complementarity of fingertip tactile sensing. While wrist force struggles with collision similarities, the fingertip iontronic film is exquisitely sensitive to subtle vibrations just as human fingers. By integrating fingertip tactile feedback, the classification accuracy for success against Type 2 failures significantly improves to 78.76%, yielding a substantial 10.06% gain. Furthermore, in a generalized binary classification task differentiating success from any failure, our dual-modal fusion framework achieves an impressive overall accuracy of 90.4%.

</div>
<div style="border: 1.5px solid #d1d5db; padding: 20px; border-radius: 10px; margin-bottom: 25px;" markdown="1">
  
<h3 style="margin-top: 0;">Automatic Material Changing System for Embedded 3D Printing of Soft Robots</h3>

*   **Overview:**  
    Soft robots typically require multi-material fabrication and need to be manufactured inside specific support materials. To address the limitations of traditional single-nozzle systems and enable automated material switching for embedded 3D printing, we developed an innovative automated material changing system featuring a simplified single-nozzle structure, optimized piston and syringe fixing mounts, and an integrated multi-nozzle motion platform.

<div align="center">
  <!-- 3D.mp4 -->
  <video width="90%" controls autoplay loop muted style="border-radius: 10px;margin-top: 10px; margin-bottom: 10px;">
    <source src="/files/3D.mp4" type="video/mp4">
  </video>
  <p style="font-size: 0.9em; color: gray;"><em>Video 2: Demo of the automated material changing 3D printer.</em></p>
</div>

*   **Design & Mechanics:**  
    We simplified the extruder structure into a compact two-part piston and syringe fixing mechanism to ensure secure attachment and easy disassembly. To achieve multi-material integration without cross-interference, we designed a single-layer horizontal switching platform driven by a three-axis motion framework and a CM35D controller, allowing the system to automatically carry, lift, and limit syringes to extrude liquid materials stably.

*   **Experiments & Results:**  
    We tested the prototype by printing multi-material planar and volumetric soft structures using silicone-based materials (such as vinyl-terminated silicone oils and crosslinkers). Experimental results demonstrate that the printer can successfully execute automated material switching and construct multi-material soft components, validating the effectiveness and feasibility of the proposed design.

*   **Key Innovations:**
    *   **Simplified Extruder Design:** Developed a streamlined, modular piston and syringe fixation mechanism that improves structural stability and simplifies component replacement.
    *   **Automated Material Switching:** Designed a multi-nozzle horizontal switching platform that enables seamless, automated transitions between different printing materials during the embedded 3D printing process.
    *   **Prototyping & Validation:** Built a complete functional prototype spanning design, fabrication, and physical testing, successfully demonstrating automated multi-material fabrication for soft robotic applications.

</div>
## Research Interests

*   🖐️ **Robotic Tactile Perception:** Developing novel biomimetic tactile sensors.
*   🧠 **Multimodal Learning:** Designing deep learning architectures and fusion strategies.
*   🦾 **Dexterous Hands:** Integrating advanced multi-modal perception systems into robotic end-effectors to achieve human-like dexterity in precision assembly.
*   🐙 **Soft Robotics:** Exploring compliant structures and materials to enhance safe physical human-robot interaction and adaptive grasping capabilities.

