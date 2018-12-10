---
layout: project
type: project
image: images/gatherLogoSquare.jpg
title: Gather - Waste Audit Web App
permalink: projects/gather
# All dates must be YYYY-MM-DD format!
date: 2018-12-09
labels:
  - JavaScript
  - Meteor
  - React
  - Web App
  - Sustainability
  - Hack-a-thon
summary: As part of a hack-a-thon challenge, our team created the Gather App to act as a centralized database that allows users to view or contribute data. 
---
<img class="ui huge floated rounded image" src="../images/gather-dashboard.jpg">
<p>
<p>As part of my final project for ICS 314 - Software Engineering I course, I participated in a hack-a-thon with the intent of creating a web app using the Meteor framework with React and MongoDB. Together with a team of six other fellow classmates, we chose to tackle the 'Trash Audit' Challenge and create an app backed by a centralized cloud database that allows users to view and contribute trash audit data.
<p>Like us, you may have never heard of a trash audit before. Basically, bags of trash are saved over a predetermined period of time. Then, on the day of the audit, the saved trash bags are opened and sorted into various categories for weighing and sometimes counting. The collected data is then put into an Excel sheet and analyzed by the University of Hawai'i at Manoa's Department of Sustainability (DoS). It's a messy job—it can't be helped—but the data collection and storage could be improved. With an app and database connected to the cloud, the data can be analyzed, visualized, and grown from anywhere by anybody with permission from the DoS. This removes the bottleneck at the administrative level and allows the DoS to scale up their endeavors effortlessly.
<p>While easy to describe, the project was difficult to implement. This is because simple, commonplace words like apps and databases are truly powerful systems that hold a lot of complexity within them—they must be implemented correctly and with care. In addition, and perhaps the greatest hurdle of all, our entire team used this project to learn the Meteor, React, and MongoDB frameworks and libraries for the first time. Thus, a considerable amount of time was spent on basics and fundamentals—no doubt a price we would not be paying if we were to start a new project with similar functionalities.
<p>During the hack-a-thon, my main roles were team leader and hardware engineer. On the team-lead side, I made extensive use of Git and GitHub to manage project code and deadlines, making sure all team members were on the same page with regards to version control protocol and project goals.
<p>For our repository protocol, a system of branches was maintained consisting of master, dev, and feature branches. Team members were only allowed to work on feature branches, and would create a pull request into the dev branch when they were done with a specific feature. The dev branch was only pulled into master for important deadlines or milestones, allowing the master branch to represent the cleanest version of our codebase up to that time.
<p>As part of our project management guidelines, we used GitHub's system for Issues, Milestones, and Projects to organize each team member's tasks and goals in a modular manner. Here, it was my job to make sure everbody kept their status up-to-date so that it would be easier for everybody to know what was going on. Also, it was my job to make sure the work would be delegated in a way that minimized team members waiting for other team members to complete a feature. After these priorities, it was my job to troubleshoot any hang-ups or delays that team members were experiencing, and shift directions when obstacles did not offer enough reward for the time spent. 
<p><img class="ui large right floated rounded image" src="../images/smartbin.jpg">On the hardware side, our team chose to create a smartbin that counted items put into it, weighed them, and sent the data to our web app as a JSON string.
