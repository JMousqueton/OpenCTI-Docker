# Welcome to OpenCTI-Docker 👋
![Version](https://img.shields.io/badge/version-1.0-blue.svg?cacheSeconds=2592000)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache2.0-yellow.svg)](#)
[![Twitter: JMousqueton](https://img.shields.io/twitter/follow/JMousqueton.svg?style=social)](https://twitter.com/JMousqueton)

> Docker-compose file to deploy OpenCTI with connectors
> 
> [OpenCTI](https://www.opencti.io) is an open source platform allowing organizations to manage their cyber threat intelligence knowledge and observables. It has been created in order to structure, store, organize and visualize technical and non-technical information about cyber threats.

## Usage

Tested on Ubuntu 20.04 

 1) git clone https://github.com/JMousqueton/OpenCTI-Docker
 2) cd OpenCTI-Docker 
 3) Modify .env file with your variables 
 4) sudo apt install docker-compose 
 5) docker-compose up -d 
 6) Wait a little and connect to http://<your_IP>:8080 

Note: 
 * Use [minio-keygen](https://github.com/JMousqueton/minio-keygen) to generate minio keygen.
 * use ``docker-compose scale worker=3`` to scale the number of workers to 3.

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
