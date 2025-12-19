---
layout: project
title: Boeing 737 Max Crashes- Ethics Analysis
description: Class project with Graphs
technologies: [MATLAB, Fusion360]
image: /assets/images/Wind_Turbine_Header.png
---
### Project Overview: Designing a custom wind turbine blade

This project focused on the design and experimental testing of a small horizontal-axis wind turbine blade optimized to maximize power extraction under a Weibull-distributed wind environment. 

### Design Process
Using the wind speed probability distribution, an effective design wind speed of **4.8 m/s** was identified as the velocity that maximizes average power output. Average extracted power was computed by weighting the turbine power at each wind speed by its probability of occurrence:

                            E[P(U)] = ∫ P(U) · p(U) dU

where P(U) is the turbine power as a function of wind speed and p(U) is the Weibull probability density function.

A MATLAB-based blade element model was developed to guide the blade design. Power extraction was modeled using the cubic dependence on wind speed

                            P(U) = (1/2) ρ A Cₚ U³

and aerodynamic forces were resolved using blade element theory. The **NACA 4412** airfoil was selected based on its favorable lift-to-drag ratio at low Reynolds numbers, with a design angle of attack of **9°**. Chord and pitch distributions were computed along the blade span to maintain this angle of attack at the selected design condition. The tangential force contributing to torque was calculated as

                     Fₜ = (1/2) ρ V²_rel c (C_L sinφ − C_D cosφ)

from which torque and power were obtained by integrating along the blade span. Iterating over candidate rotational speeds while enforcing stress, torque, and RPM limits resulted in a final **design RPM of 1050**, with a predicted maximum power output of **3.61 W** at **4.82 m/s**.

![Experimental vs. Actual Data]({{ "/assets/images/Power_Curves.png" | relative_url }}){: .inline-image-r style="width: 1200px"}

### Testing Summary

The fabricated turbine was tested in a wind tunnel at five wind speeds ranging from **4.1 m/s to 5.8 m/s**. Experimental results showed that the turbine consistently operated at higher rotational speeds than predicted, with an experimentally determined optimal operating speed of **1770 RPM**. The maximum measured power output was **1.8 W at 5.8 m/s**.

---

| Wind Speed (m/s) | Predicted Max Power (W) | Experimental Max Power (W) | % Error |
|:----------------:|:----------------------:|:--------------------------:|:-------:|
| 4.8 (design)     | 3.61                   | 0.70                       | 81%     |
| 5.8 (max tested) | 6.50                   | 1.80                       | 72%     |

---


Although the turbine underperformed relative to analytical predictions, the results validate the overall blade design methodology and demonstrate the effectiveness of optimizing blade taper, twist, and lift-to-drag ratio under probabilistic wind conditions. Discrepancies between modeled and experimental performance are attributed to simplifying assumptions such as constant induction factors, neglected tip losses, and unmodeled friction.



![Experimental vs. Actual Data]({{ "/assets/images/Experimental_Actual.png" | relative_url }}){: .inline-image-r style="width: 1200px"}

### My Contribution
Design process: optimizing pitch and taper in MATLAB, experimental test protocol, data processing and results

![Experimental vs. Actual Data]({{ "/assets/images/Wind_Turbine.png" | relative_url }}){: .inline-image-l style="width: 1200px"}