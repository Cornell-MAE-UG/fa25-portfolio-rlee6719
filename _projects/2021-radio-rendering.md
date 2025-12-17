---
layout: project
title: Wind Turbine Blade
description: MAE 4727 - Design, Analysis, Testing of a Wind Turbine Blade
technologies: [Autodesk Inventor, MATLAB]
image: /assets/images/render.png
---

Project overview: 
For MAE 4272 Fluids and Heat Transfer Laboratory we designed and tested a small scale wind turbine blade to maximize power generation under a given wind speed distribution and comply with geometric, operational and structural constraints. The primary design challenge was in selecting an appropriate airfoil and defining the pitch angle and chord of the blade in a way that ensured the structural integrity of the blade under test conditions. I worked on developing the analysis, design and testing of the part and was responsible for the 3D modeling of the wind turbine blade in Autodesk Inventor along with testing.

![Blade 3D Render]({{ "/assets/images/render.png" | relative_url }}){: .inline-image-l}

Our design process began by defining an effective global wind speed from the given Weibull distribution using an integration based method that accounts for realistic variability in operations. We then selected a target operating point factoring in the tip speed ratio which resulted in a design rotation rate of 1400 RPM which is within our design constraints. Using a weighted spanwise analysis we determined from this point that the effective Reynolds number would be approximately 17000. 

![Windspeed Analysis]({{ "/assets/images/windspeed.png" | relative_url }}){: .inline-image-l}

Given that most available data online for airfoils used significantly higher Reynolds numbers, we applied scaling relations to adjust the lift and drag coefficient to match our relatively low operating range. Using this approach, we identified a number of candidate airfoils to compare based on efficiency and robustness to angle of attack variations. This yielded the SD7037 airfoil which proved to be the most reliable in our operating conditions. The ideal blade pitch and chord distributions were found using mathematical models provided from the Wind Power class. With this final geometry in hand we conducted a structural analysis of the blade that confirmed that it would not fail under the expected loads. 

![Airfoil Analysis]({{ "/assets/images/airfoil.png" | relative_url }}){: .inline-image-l}

Testing summary: Our blades were tested in a wind tunnel to generate power curves at several wind speeds following the procedure outlined below. 

![Test Procedure]({{ "/assets/images/testing.png" | relative_url }}){: .inline-image-l}

While we were able to collect data at a couple of wind speeds that generally exhibited the shape of the expected power curve, our measured power output was significantly lower than what was analytically predicted. This discrepancy can be attributed to a number of factors such as higher friction, resonance effects, wake interactions and a CAD error that resulted in the blade profile being mirrored across the chord. Although we were not able to collect data that necessarily validated our analytical models, these findings did point us in the right direction towards improving our models and assumptions in the future. 

![Power curves]({{ "/assets/images/powercurve.png" | relative_url }}){: .inline-image-l}
