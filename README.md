# Welcome to OpenCTI-Docker 👋
![Version](https://img.shields.io/badge/version-4.5.0-blue.svg?cacheSeconds=2592000)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache2.0-yellow.svg)](#)
[![Twitter: JMousqueton](https://img.shields.io/twitter/follow/JMousqueton.svg?style=social)](https://twitter.com/JMousqueton)

> Docker-compose file to deploy OpenCTI with connectors
> 
> [OpenCTI](https://www.opencti.io) is an open source platform allowing organizations to manage their cyber threat intelligence knowledge and observables. It has been created in order to structure, store, organize and visualize technical and non-technical information about cyber threats.

## Information 

- This Docker-compose file include the following OpenCTI connectors : 

| Name | Request a token/api key |
| ------- | ------------------ |
| Common Vulnerabilities and Exposures | :x: |
| VirusTotal | :white_check_mark: |
| MITRE ATT&CK | :x: |
| OpenCTI | :x: |
| Cybercrime-Tracker (ANSSI) | :x: |
| CyberThreatCoalition | :x: |
| AM!TT | :white_check_mark: |
| AlienVault | :white_check_mark: |
| AbuseIPDB | :white_check_mark: |
| Valhalla | :white_check_mark: |
| Abuse.ch URLhaus | :x: |
| Malbeacon  | :white_check_mark: |
| greynoise  | :white_check_mark: |
| Hybrid Analysis Sandbox | :white_check_mark: |
| Sekoia | :white_check_mark: | 

- [Changelog](https://github.com/JMousqueton/OpenCTI-Docker/blob/main/CHANGELOG.md)

## Usage

Tested on Ubuntu 20.04 

 1) ``git clone https://github.com/JMousqueton/OpenCTI-Docker``
 2) ``cd OpenCTI-Docker``
 3) Modify .env file with your variables 
 4) ``sudo apt update; sudo apt upgrade; sudo apt install docker-compose``
 5) ``docker-compose up -d`` 
 6) Wait a little and connect to http://<your_IP>:8080 

Note: 
 * Use [minio-keygen](https://github.com/JMousqueton/minio-keygen) to generate minio keygen.
 * use ``docker-compose scale worker=3`` to scale the number of workers to 3.

## Upgrade 

 1) ``cd OpenCTI-Docker``
 2) ``git pull`` 
 3) ``docker-compose pull`` 
 4) ``docker-compose up -d``  

## Scale 

You can scale the number of worker up to 3.

In the OpenCTI directory : 

* ``docker-compose scale worker=3`` 

## References 
 
 * OpenCTI: https://www.opencti.io 
 * OpenCTI (sources): https://github.com/OpenCTI-Platform/opencti
 * OpenCTI (Docker sources): https://github.com/OpenCTI-Platform/docker
 * OpenCTI (Connectors sources): https://github.com/OpenCTI-Platform/connectors

## Author

👤 **Julien Mousqueton**

* Website: https://www.julienmousqueton.fr
* Twitter: [@JMousqueton](https://twitter.com/JMousqueton)
* Github: [@JMousqueton](https://github.com/JMousqueton)
* LinkedIn: [@julienmousqueton](https://linkedin.com/in/julienmousqueton)
* CV: https://jmousqueton.github.io

## Show your support

Give a ⭐️ if this project helped you!
