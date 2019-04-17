---
layout: project
type: project
image: images/office.jpg
title: AmbiProxiLITE - Ambient Proximity Lighting
permalink: projects/ambiproxilite 
# All dates must be YYYY-MM-DD format!
date: 2018-12-09
labels:
  - Node-RED
  - JavaScript
  - IBM Cloud
  - Raspberry Pi
  - Sense HAT
  - IoT
  - Beacons
summary: . 
---
<p>For my group's final project in EE 491E, we decided to implement an IoT solution that uses Bluetooth "beacons" to control office lights to turn on only when a beacon is close to the work area. The dream is to create a scalable model for buildings that will allow electricty to be conserved when rooms are not in use. By having a small beacon on keychains or badges of employees, the proximity system will know what part of a building is being used and adjust the lights accordingly. Data on office and light usage can help administrative personnel better understand their energy usage, office layout, and other data that could potentially provide evidence of restructuring of workspaces or office procedures for further efficiency improvements.
<p>We are simulating this system using a Raspberry Pi, Sense HAT, and Estimote Beacon. The Raspberry Pi will act as the detector, sensing any beacons and their distance from the Pi using Bluetooth. 
<p><img class="ui large right floated rounded image" src="../images/estimote.jpg">estimote beacon descrip.
<p><img class="ui large left floated rounded image" src="../images/rpi.jpg">rpi/nodered descrip
