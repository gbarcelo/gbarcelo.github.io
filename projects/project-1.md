---
layout: project
type: project
image: images/proj1_1.jpg
title: Reinforcement Learning with Arduino Slave Agent
permalink: projects/rl_arduino
# All dates must be YYYY-MM-DD format!
date: 2017-12-12
labels:
  - Machine Learning
  - Reinforcement Learning
  - Arduino
  - C++
  - Python
summary: Reinforcement Learning with Microcontroller Slave Agent
  - Proposed, designed, and developed a quadrupedal robot that learns to walk in a direction using a neural network observing leg states/actions and distance measurements
  - Applied Arduino technologies, Bluetooth, TensorFlow, Python, and C/C++
---
The project team consisted of myself and my partner Ryan Ganiron. My roles in the project were the following:

Project/Design Lead:
I proposed and designed a master/slave system to learn how to walk without any movements being explicitly programmed. The master was a neural network on a PC written using TensorFlow’s machine learning library. The slave was a quadrupedal robot controlled by an Arduino microcontroller board. The master and slave communicated serially via Bluetooth, with the master receiving leg state and distance data from the slave and sending new leg states (i.e. actions) back to the slave to execute.
These decisions were made because we initially could not find a way to place neural network software onto the Arduino microcontroller, and the physical weight of a wired connection adversely affected the mobility of the robot unit. Leg state and distance data served as inputs for our neural network agent in learning how to combine various leg movements to accomplish a net forward movement.
 
Software Lead:
I wrote most of the software in this project, and I checked and debugged all of it. The software has three main parts: the neural network agent script, the master/slave serial protocol script, and the Arduino microcontroller script.
The neural network agent Python script was written by me and acted as the main control of the system and handled the actual learning. The agent was instantiated here and went through a large number of training iterations, updating itself every fixed interval based on rewards given on state-action conditions. After training, the saved model variables could be executed based on what the agent learned as the most valuable action when in a given state.
The master/slave serial protocol script was written by me in Python and acted as the bridge between the master and slave. It was developed according to the current convention in machine learning problems. For example, when the agent script calls for an environment step env.step(a), the protocol script will take the action a and signal the robot slave via Bluetooth to execute the action and report back the state and a smoothed distance reading. In this way, the protocol script took care of most of the menial tasks and acted as a preprocessing unit and catch-all for data and control. For example, when the slave unit provides a distance reading, the protocol script would then decide if a reward value of 1 or 0 should be returned to the agent script after a given step.
The Arduino microcontroller script was written by Ryan Ganiron in C initially, but due to troubleshooting and design iterations was heavily edited by me. This script handled moving the servos (legs) of the robot with a time delay, taking smoothed distance readings (an average of 10), and maintaining its own Bluetooth module and communications.
 
Hardware/Mechanical Integrator:
        	I took the hardware circuit and materials implemented and provided by Ganiron and designed and implemented a basic quadrupedal unit to support it. The chassis and legs were made of balsa wood, wire, and glue, and the hardware components were secured using zip ties. The wood and zip ties were used in order to facilitate dexterity in the face of any possible required design changes. Wire and glue were used to strengthen critical or structurally weak areas of the unit.




