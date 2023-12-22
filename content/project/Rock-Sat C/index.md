---
title: Rock-Sat C Student Launch Opportunity
summary: Student launch opportunity investigating plasma in the upper ionosphere. Cool rocket stuff. Fall 2022 - Summer 2023.
tags:
 - Featured
 - DSpOC
 - Instrumentation

image:
 caption: Photo of Payload at Flight Integration

show_date: false
---

As a follow-up to my Rock-On experience, I participated in the annual Rock-Sat C student launch opportunity, again as a University of Delaware team member. Unlike Rock-On, though, we were designing a novel experiment and scientific payload from scratch. My group chose a Langmuir Probe, one of the few experiments capable of producing novel data in the upper ionosphere, the peak height of our sub-orbital sounding rocket.

A Langmuir Probe essentially turns plasma into a big ol' resistor. By applying an electric potential (voltage difference) between two points separated by plasma and measuring the current induced, you can fit the result to an equation to find the temperature and density of the plasma (Figure 1). As an in-situ device, a Langmuir Probe would be an excellent candidate for producing data on a sounding rocket, where we spend most of our time in the ideal environment.

{{< figure src="Langmuir Probe Demo.png" caption="Example of a Langmuir Probe in use" numbered="true" >}}

My work was in the sampling electronics, flight software, and ground software that collected, packaged, and analyzed the data, respectively.

My primary role was ground software lead, where I used a custom graphical user interface to parse data, fit and analyze it, and match it to sensor data. The ground software was Python-based and used the prior library work done by previous teams. Using old data, my software was developed to plot, compare, and fit all 4,000+ samples. Useful features include a composite graph system that merges data from all three gain levels to create the highest possible accuracy plot, sample searching that finds samples that match the requested temperature or density, and outlier/noise/hysteresis mitigation. Additionally, the ground software developed was used to optimize sampling techniques to allow higher precision and speed in flight.

{{< figure src="Ground Software.png" caption="Screenshot of the developed graphical interface with data from previous years displayed." numbered="true" >}}

My secondary roles were to assist in developing the flight software and analog electronics. Working alongside the leads for each subsystem, I assisted in system integration, PCB design, data collection, and mechanical design. To mitigate the noise and hysteresis seen in previous-years data, a new electronics implementation was developed, where we would put our trans-impedance and differential amplifiers in the port with the probe on a low-profile board (Figure 2). This would allow all critical processing to be done right next to our experiment rather than in our payload canister several meters away. For flight software, I assisted in optimizing sampling patterns using insights gained from ground software development.

{{< figure src="Analog Block Diagram.png" caption="Functional block diagram of the analog data sampling sub-system. The dotted section was placed in the external port with our probe, while the rest remained in the payload canister." numbered="true" >}}

Our project culminated in a launch in August 2023. Unfortunately, due to an oversight in the design of the power system, our team lost power after reaching maximum thrust. No useful data was recovered. All future development of the University of Delaware Ionospheric Probe and the ground software has been handed off to the Delaware Cube-Sat team, who will tentatively launch in Spring 2025.

{{< youtube xMIaCJXXrcI >}}

Great thanks to Professor Maruca and Jarod Dagney, who were the project advisors and my personal mentors. Additionally, Dax Moreas, thank you for being an incredible team leader, and it was a pleasure to work with Nick Ulizio, TJ Kaifer, Miguel Mercado, and Allie Phantom. Finally, this project was only possible with the financial support of the Delaware Space Grant Consortium and the Wallops Island Flight Facility’s educational team.

{{< figure src="Gang.jpg" caption="It was a blast, gang. (L-R) Miguel, Allie, Nick, Me, Dax, Dr. Maruca, TJ, Jarod." numbered="true" >}}