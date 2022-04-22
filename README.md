# Hight Diploma Computer Science 2020 Project

- Student: Alvaro Sanchez Domingo
- Student Number: 20091387
- Date: 18-04-2022
- Project Name: Lynx Monitoring
- Project Title: An Industry 4.0 system for automated machinery and production lines monitoring

# Abstract
Lynx monitoring is an application deployed in a physical PC on-site. It takes data from industrial machines and distils the information into an integrated dashboard to allow the end-user to monitor and analyse real time and historic key performance indicators of automated production lines. Thus, quicker, better and more efficient decisions can be made. This industry digitalization, or so-called Industry 4.0, is becoming more and more essential every day. This system has been designed for a machine manufacture company called AND&OR to digitalize its current products, add value to them and supply to its customers with a better product.

# Project Image

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/project_image.png">

# Project Links

- Jira Project Gantt Chart

https://asanchez.atlassian.net/jira/software/projects/WP/boards/1/roadmap?shared=&atlOrigin=eyJpIjoiYWJkYWI1NDVkMzUyNDk2Yjk5YjgzMWNhYjcyYzc5MDciLCJwIjoiaiJ9

 - Project video

 https://www.youtube.com/watch?v=hX1NuaEbJF0
 
# Project code

- Front End (Svelte) Confidential information

https://github.com/AlvaroSanchezDomingo/lynx-front-end


- Database Service (Node.js) Confidential information

It is a service program deployed in Node.js that manages the interaction with the data base. This service exposes API REST endpoints so that other services or front end can interact with it in order to request or manage data of users, machines, sections, devices, alarms, shifts, etc.

https://github.com/AlvaroSanchezDomingo/lynx-db-service


- Time Series Service (Node.js) Confidential information

It is a service program deployed in Node.js that manages the interaction with the time series database. This service is subscribed to all the topics of the message broker, which manages the intake of variables, in order to store production data accordingly. This service exposes API REST endpoints so that other services or front end can interact with it in order to request and manage production data.

https://github.com/AlvaroSanchezDomingo/lynx-ts-service

- Cache service (Node.js) Confidential information

It is a service program deployed in Node.js that manages the interaction with the in-memory database. This service is subscribed to all the topics of the message broker, which manages the intake of variables, in order to store the current value of all variable. This service exposes API REST endpoints so that other services or front end can interact with it in order to request current data.

https://github.com/AlvaroSanchezDomingo/lynx-cache-service

- Engine Service (Node.js) Confidential information

It is a service program deployed in Node.js that run processes in the background such as decoding alarms or perform heavy calculations. This service interacts with other services via API REST to retrieve information from the different databases, analyse it and serve it via API REST. This service is subscribed to alarm topics of the message broker so that alarms can be decoded and processed.

https://github.com/AlvaroSanchezDomingo/lynx-engine-service

- Cloud Service (Node.js) Confidential information

It is a service program deployed in Node.js that manages the upload of data to the cloud. This service is subscribed to all the topics of the message broker, which manages the intake of variables, in order to upload production data to the cloud accordingly.

https://github.com/AlvaroSanchezDomingo/lynx-cloud-service

- Data Capture Service (Node-Red) Confidential information

It is a service program deployed in Node-RED that manages the capture of data from production machinery using standard industrial protocols such as Modbus-TCP and it is in charge of publishing this information to the rest of the services via the message broker.

https://github.com/AlvaroSanchezDomingo/lynx-node-red

- Deployment (Docker) Confidential information

https://github.com/AlvaroSanchezDomingo/lynx-docker



# Application

- Login

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/login.png">

- Plant dashboard

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/plant.png">

- Line running dashboard

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/line_running.png">

- Line stopped dashboard

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/line_stopped.png">

- Machine dashboard

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/machine_main.png">

- Machine status dashboard

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/machine_status.png">

- Machine production dashboard

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/machine_production.png">

- Machine alarms dashboard

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/machine_alarms.png">

- Device list

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/device_list.png">

- Device configuration

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/configuration_device.png">

- Machine list

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/machine_list.png">

- Machine configuration

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/configuration_machine.png">

- Section list

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/section_list.png">

- Section configuration

<img src="https://github.com/AlvaroSanchezDomingo/hdip_computer_science_project/blob/master/images/configuration_section.png">