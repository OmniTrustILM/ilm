# Welcome to CZERTAINLY!

![CZERTAINLY-logo](czertainly-logo/czertainly_color_H.svg)

CZERTAINLY is a platform for effective and efficient trust lifecycle management for companies of any size and individuals. One of its goals is to provide an easy and affordable way to secure digital communication and support information security in more and more connected world.

CZERTAINLY is released as a commercial open source project under the [MIT License](LICENSE.md).
Additional features and services are available under subscription plans. If you are interested in subscription, please contact us through [CZERTAINLY Official Web](https://www.czertainly.com) or use the [CZERTAINLY Offical email address](mailto:info@czertainly.com) email address.

CZERTAINLY is designed and developed by a team of PKI and information security enthusiasts with practical point of view on the certificate management in hybrid environments. PKI is the backbone of security in our daily communication and its security and easy management should be available to everyone.

## CZERTAINLY features

The CZERTAINLY platform aims to provide easy, secure, and extensible features for certificate management. Among the features are:
- certificate management (issuing, revocation, renewal) through RA Profile and standard protocols
- cryptographic key management (generation, encryption, signing, etc.) through Token Profile
- extensible connectors to support many technologies and implementations of certification authorities, credentials, discovery engines, cryptography, compliance, and more
- certificate searching in various sources
- consistent inventory of certificates and cryptographic keys (owners, groups, entities, profiles, and more)
- dashboard for monitoring and reporting

## About the platform

The platform is split into several components:
- interfaces (UIs, REST API, etc.)
- authentication and authorization
- core services provided by the platform (discovery, inventory, connectors, authorities, tokens, etc.)
- grouping and entity automation
- data storage
- connectors and functional groups and types (discovery provider, ca connector, credential provider, cryptography provider etc.)

Components in the platform act as microservices and the main approach is to keep each service as a simple container. 

## Repositories

| Repository                                                                                  | Description                                                                                                                                                                                         |
|---------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [CZERTAINLY-Interfaces](https://github.com/CZERTAINLY/CZERTAINLY-Interfaces)               | Interfaces to build custom connectors and extend the platform. Each interface is build as a REST API and you can use any technology for building your own extension you like                        |
| [CZERTAINLY-Core](https://github.com/CZERTAINLY/CZERTAINLY-Core)                           | Core services of the platform. This is the brain of the platform taking care about all operations with certificates and managing the connection between different types of connector implementations |
| [CZERTAINLY-Auth](https://github.com/CZERTAINLY/CZERTAINLY-Auth)                           | Auth service is designed as a central service for managing access control to different resources and related actions and objects, and identify users based on identification token                  |
| [CZERTAINLY-Auth-OPA-Policies](https://github.com/CZERTAINLY/CZERTAINLY-Auth-OPA-Policies) | OPA policies for external evaluation of Auth service permissions served for OPA                                                                                                                     |
| [CZERTAINLY-Scheduler](https://github.com/CZERTAINLY/CZERTAINLY-Scheduler)                 | Scheduler service is designed to manage the automation of executed tasks                                                                                                                            |
| [CZERTAINLY-Documentation](https://github.com/CZERTAINLY/CZERTAINLY-Documentation)         | Documentation of the platform containing also information for contributors and developers                                                                                                           |
| [CZERTAINLY-FE-Administrator](https://github.com/CZERTAINLY/CZERTAINLY-FE-Administrator)   | Administrator web interface to manage platform and lifecycle of trust services                                                                                                                      |

### Providers and Connectors

| Repository                                                                                                            | Description                                                                           |
|-----------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------|
| [CZERTAINLY-Common-Credential-Provider](https://github.com/CZERTAINLY/CZERTAINLY-Common-Credential-Provider)         | Common credential provider that allows to work with basic credentials in the platform |
| [CZERTAINLY-EJBCA-NG-Connector](https://github.com/CZERTAINLY/CZERTAINLY-EJBCA-NG-Connector)                         | Authority and discovery provider for [EJBCA](https://www.ejbca.org/)                  |
| [CZERTAINLY-MS-ADCS-Connector](https://github.com/CZERTAINLY/CZERTAINLY-MS-ADCS-Connector)                           | Authority and discovery provider for MS ADCS                                          |
| [CZERTAINLY-PyADCS-Connector](https://github.com/CZERTAINLY/CZERTAINLY-PyADCS-Connector)                             | Authority and discovery provider for MS ADCS using Python                             |
| [CZERTAINLY-X509-Compliance-Provider](https://github.com/CZERTAINLY/CZERTAINLY-X509-Compliance-Provider)             | Compliance provider for X.509 certificates                                            |
| [CZERTAINLY-IP-Discovery-Provider](https://github.com/CZERTAINLY/CZERTAINLY-IP-Discovery-Provider)                   | Network discovery provider for internal and external networks                         |
| [CZERTAINLY-Cryptosense-Discovery-Provider](https://github.com/CZERTAINLY/CZERTAINLY-Cryptosense-Discovery-Provider) | Discovery provider integrated with Cryptosense Analyzer                               |
| [CZERTAINLY-Keystore-Entity-Provider](https://github.com/CZERTAINLY/CZERTAINLY-Keystore-Entity-Provider)             | Entity provider for managing certificates in Java Keystores                           |
| [CZERTAINLY-Software-Cryptography-Provider](https://github.com/CZERTAINLY/CZERTAINLY-Software-Cryptography-Provider) | Cryptography provider for managing cryptographic keys in software keystores           |
| [CZERTAINLY-Email-Notification-Provider](https://github.com/CZERTAINLY/CZERTAINLY-Email-Notification-Provider)       | Email notification provider for sending notifications                                 |

### Supporting repositories

| Repository                                                                      | Description                                    |
|---------------------------------------------------------------------------------|------------------------------------------------|
| [CZERTAINLY-Helm-Charts](https://github.com/CZERTAINLY/CZERTAINLY-Helm-Charts) | Helm charts to install and maintain CZERTAINLY |
| [CZERTAINLY-Appliance](https://github.com/CZERTAINLY/CZERTAINLY-Appliance)     | CZERTAINLY virtual appliance                   |

### Other

| Repository                                                                                    | Description                                                                |
|-----------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
| [CZERTAINLY-Keycloak-Theme](https://github.com/CZERTAINLY/CZERTAINLY-Keycloak-Theme)         | CZERTAINLY custom Keycloak theme                                           |
| [CZERTAINLY-Keycloak-Optimized](https://github.com/CZERTAINLY/CZERTAINLY-Keycloak-Optimized) | Optimized Keycloak for CZERTAINLY platform                                 |
| [CZERTAINLY-Dependencies](https://github.com/CZERTAINLY/CZERTAINLY-Dependencies)             | Helper dependecies for CZERTAINLY component using `Java` and `Spring Boot` |
| [CZERTAINLY-Utils-Service](https://github.com/CZERTAINLY/CZERTAINLY-Utils-Service)           | Helper service for CZERTAINLY components                                   |

## Contribution

Anyone can contribute to CZERTAINLY and we would be happy to support you in that. See [Contribution Guide](CONTRIBUTING.md) for more information.

## License

The CZERTAINLY platform is released under the [MIT License](LICENSE.md). Some connectors and user interfaces are released under their own licenses or subscriptions. Consult with us for more information.
