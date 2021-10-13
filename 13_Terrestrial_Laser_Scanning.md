# Terrestrial Laser Scanning (TLS)
---

## Content

*Just jump to the topic you are looking for*

- [Introduction](#introduction)
- [Range](#range)
- [XYZ Coordinates](#xyz-coordinates)
- [Shading](#shading)
- [Multiple Scan Positions](#multiple-scan-positions)
- [Moving Objects](#moving-objects)

---

## Introduction

>There are two main types of laser scanning technologies. The Mobile Laser Scanning (MLS) and the Terrestrial Laser Scanning (TLS). The mobile laser scanning is a laser which is mounted to a moving vehicle or an airplane (ALS: Airborne Laser Scanning). It is used to survey large areas like landscapes, cityscapes etc.
>The terrestrial laser scanning is more stationery and ground based, in comparison to the moving method. The scanner is mounted on a tripod and can measure points around his own axis. This type often produces more detailed point clouds than the MLS or ALS method, but in a much smaller scale.
>Besides the differences, both methods are using a laser to measure distance trough light and time.

![TLS_1](/doc/TLS_1.png)

## Range

>We will focus on the terrestrial lasers, which are mounted on a tripod. Different types of lasers have different ranges. The Riegl Laser scanner for example can reach up to 6 km, and for that is called a Long-Range-Laser-Scanner. Compared to that, the smaller Faro Laser Scanner has a range up to 350 m, which puts it in the category of Short-Range-Laser-Scanner. The range strongly depends on the chosen model.

![TLS_2](/doc/TLS_2.png)

>The Laser shots millions of laser beams per second in a predefined grid in all direction (360° horizontal and 240° vertically) there is some non-measured space underneath the scanner where it is mounted to the tripod. The grid is the resolution of your point cloud. The higher the resolution, the closer are the points.

## XYZ Coordinates

>The scanner measures the time the light needs to travel to the closest surface and back, and then calculates the distance due to the needed amount of time. Then safes for each point the XYZ coordinate in a relative position to the scanner origin (optional linked with an GPS coordinate). As well as the color information (RGB) from a photo, which is taken automatically by the scanner after the scan process. And finally, the intensity of the light that has been reflected (number from 1-256). The Intensity value can be used for example to land cover classification (water reflects the laser beam different from a leaf). All this point information is then later used to register and connect all the different scans from all the positions to each other to get a complete point cloud.

![TLS_3](/doc/TLS_3.png)

## Shading

>In praxis, the range is often not the limiting factor of the scanner. In an urban environment or on an open field there are most of the time obstacles like cars, trees or buildings which are blocking the light. This phenomenon is called “Shading”. The laser can’t see through these objects. So, it will measure the distance to and from the obstacle and everything behind is left as an unknown empty space (shadow) without data information. The closer such an obstacle is, the more it blocks your scan. So be careful by choosing your scan location.

![TLS_4](/doc/TLS_4.png)

## Multiple Scan Positions

>The solution to that is to take multiple scans from different position with a certain overlap by moving the scanner. It is then possible to see “behind” the obstacle or around a corner that was before blocking the laser beam. Later in the point cloud registration software, you can then eliminate the overlapping points, as well as cover the black shadows from one scan with another.

![TLS_5](/doc/TLS_5.png)

## Moving Objects

>While scanning, be aware of moving objects. A moving car or a person that moves with the rotation of the laser can also block the laser and results in a useless laser scan.
>On the other hand, a person or a vehicle crossing the laser beam only briefly has hardly any influence on the final scan. Only a few points of the object are registered and then referenced with the photo at the end, so the points of the object then have the color of the surrounding. The reverse is somewhat more disturbing. If a moving object crosses the scanner during the photo process, the points from the surrounding are later superimposed with the photo of the object.

![TLS_6](/doc/TLS_6.png)
