# Welcome to OpenCTI-Docker 👋

![Version](https://img.shields.io/badge/version-5.3.7-blue.svg?cacheSeconds=2592000)
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
| Cybercrime-Tracker | :x: |
| ~~CyberThreatCoalition~~ | source ended in Nov '21 |
| AM!TT | :white_check_mark: |
| AlienVault | :white_check_mark: |
| AbuseIPDB | :white_check_mark: |
| Abuse.ch URLhaus | :x: |
| Malbeacon  | :white_check_mark: |
| CryptoLaemus | :x: |
| Shodan | :white_check_mark: |
| Malpedia | :x: |

- [Changelog](CHANGELOG.md)

## Usage

Tested on Ubuntu 20.04

 1) ``git clone https://github.com/JMousqueton/OpenCTI-Docker/``
 2) ``cd OpenCTI-Docker``
 3) ``cp .env.sample .env``
 4) Modify .env file with your variables
 5) ``sudo apt update && sudo apt upgrade -y && sudo apt install docker-compose``
 6) ``sudo docker-compose --profile start up -d``
 7) Wait a little and connect to http://<your_IP>:8080

Note:

- Use [minio-keygen](https://github.com/JMousqueton/minio-keygen) to generate minio keygen.
- use ``uuid-gen`` to generate TOKEN and connectors ID.

## Scale

You can scale the number of worker up to X.

In the OpenCTI directory :

- ``docker-compose scale worker=X``

## Upgrade

 1) ``cd OpenCTI-Docker``
 2) ``git pull``
 3) ``docker-compose pull``
 4) ``docker-compose up -d``  

Note:

- To only update OpenCTI version, you can replace step 1 & 2 by editing the first line of .env with the targeted version.

## References

- OpenCTI: <https://www.opencti.io>
- OpenCTI (sources): <https://github.com/OpenCTI-Platform/opencti>
- OpenCTI (Docker sources): <https://github.com/OpenCTI-Platform/docker>
- OpenCTI (Connectors sources): <https://github.com/OpenCTI-Platform/connectors>

## Author

👤 **Julien Mousqueton**

- Website: <https://julienm.io>
- Twitter: [@JMousqueton](https://twitter.com/JMousqueton)
- Github: [@JMousqueton](https://github.com/JMousqueton)
- LinkedIn: [Julien Mousqueton](https://linkedin.com/in/julienmousqueton)
- CV: <https://jmousqueton.github.io>

## Show your support

Give a ⭐️ if this project helped you!
