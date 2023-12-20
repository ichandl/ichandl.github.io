---
title: Rock-Sat C Student Launch Opportunity
summary: Student launch opportunity, investigating plasma physics in the upper ionosphere.
tags:
 - Featured
 - DSpOC
 - Instrumentation

image:
 caption: Photo of Payload at Flight Integration

show_date: false
---

As a follow up to my [Rock-On experience]({{< relref "../rock-on-workshop/" >}}), I participated in the annual Rock-Sat C student launch opportunity, again as a member of the University of Delaware Team. Unlike Rock-On though, this time we were designing an experiment and scientific payload from scratch. My group chose a Langmuir Probe, as it was one of the few experiments capable of producing novel data in the upper ionosphere, the peak hight of our sub-orbital sounding rocket.

A Langmuir Probe essentially turns plasma into a big ol' resistor. By applying an electric potential (voltage difference) between two points seperated by plasma, and measuring the current induced, you can fit the result to an equation to find the temperature and density of the plasma. As an in-situ device, a Langmuir Probe would be an excellent candidate for producing data on a sounding rocket, where we spend most of our time in the ideal environment.

{{< figure src="Langmuir Probe Demo.png" caption="Example of a Langmuir Probe in use" numbered="true" >}}

My work was in the sampling electronics, flight software, and ground software that collected the data, packaged it, and analysed it, respectively. 

My primary role was ground software lead, where I used a custom graphical user interface to parse data, fit and analyze it, and match it to sensor data. 
