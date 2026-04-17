# Welcome to ILM!

![ILM-logo](logo/ot-color.svg)

ILM (Identity Lifecycle Management) is a platform for effective and efficient trust lifecycle management for companies of any size and individuals. One of its goals is to provide an easy and affordable way to secure digital communication and support information security in more and more connected world.

ILM is released as a commercial open source project under the [MIT License](LICENSE.md).
Additional features and services are available under subscription plans. If you are interested in subscription, please contact us through [OmniTrust Official Web](https://www.omnitrust.com) or use the [ILM Official email address](mailto:ilm@omnitrust.com) email address.

ILM is designed and developed by a team of PKI and information security enthusiasts with practical point of view on the certificate management in hybrid environments. PKI is the backbone of security in our daily communication and its security and easy management should be available to everyone.

## Documentation

For comprehensive documentation, visit [docs.otilm.com](https://docs.otilm.com).

## ILM features

The ILM platform aims to provide easy, secure, and extensible features for certificate and identity lifecycle management. Among the features are:
- certificate management (issuing, revocation, renewal) through RA Profile and standard protocols
- cryptographic key management (generation, encryption, signing, etc.) through Token Profile
- secrets management (passwords, API keys, JWT tokens, cryptographic keys, keystores, key-value pairs) through Vault Profile with versioning, cross-vault synchronization, approval workflows, and compliance evaluation
- cryptographic bill of materials (CBOM) scanning and repository
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
- connectors and functional groups and types (discovery provider, CA connector, credential provider, cryptography provider, etc.)

Components in the platform act as microservices and the main approach is to keep each service as a simple container.

## Repositories

### Core Platform

| Repository                                                             | Description                                                                  |
|------------------------------------------------------------------------|------------------------------------------------------------------------------|
| [core](https://github.com/OmniTrustILM/core)                           | Core of the platform managing certificate lifecycle management related tasks |
| [auth](https://github.com/OmniTrustILM/auth)                           | Authentication service for the platform                                      |
| [auth-opa-policies](https://github.com/OmniTrustILM/auth-opa-policies) | OPA policies for evaluating access control permissions                       |
| [scheduler](https://github.com/OmniTrustILM/scheduler)                 | Scheduler of activities and tasks                                            |
| [interfaces](https://github.com/OmniTrustILM/interfaces)               | Interface definitions and common objects for the platform                    |
| [utils-service](https://github.com/OmniTrustILM/utils-service)         | Utils service to support various certificate and key handling                |
| [dependencies](https://github.com/OmniTrustILM/dependencies)           | Common dependencies for Java projects                                        |

### User Interfaces

| Repository                                                           | Description                 |
|----------------------------------------------------------------------|-----------------------------|
| [fe-administrator](https://github.com/OmniTrustILM/fe-administrator) | Administrator web interface |

### CBOM (Cryptographic Bill of Materials)

| Repository                                                         | Description                                                                                                        |
|--------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| [cbom-lens](https://github.com/OmniTrustILM/cbom-lens)             | CLI tool to scan filesystems, containers, and network ports for cryptographic assets and generate a CycloneDX CBOM |
| [cbom-repository](https://github.com/OmniTrustILM/cbom-repository) | Repository for uploading, retrieving, and searching CBOM documents                                                 |

### Providers and Connectors

| Repository                                                                                       | Description                                                   |
|--------------------------------------------------------------------------------------------------|---------------------------------------------------------------|
| [common-credential-provider](https://github.com/OmniTrustILM/common-credential-provider)         | Common credential provider for working with basic credentials |
| [ejbca-ng-connector](https://github.com/OmniTrustILM/ejbca-ng-connector)                         | EJBCA NG connector for certificate management and discovery   |
| [pyadcs-connector](https://github.com/OmniTrustILM/pyadcs-connector)                             | Connector for MS ADCS using Python                            |
| [hashicorp-vault-connector](https://github.com/OmniTrustILM/hashicorp-vault-connector)           | Connector to HashiCorp Vault PKI secrets engine               |
| [x509-compliance-provider](https://github.com/OmniTrustILM/x509-compliance-provider)             | Compliance provider for X.509 certificates                    |
| [ip-discovery-provider](https://github.com/OmniTrustILM/ip-discovery-provider)                   | Discovery provider to identify certificates on network        |
| [cryptosense-discovery-provider](https://github.com/OmniTrustILM/cryptosense-discovery-provider) | Discovery provider for Cryptosense Analyzer reports           |
| [ct-logs-discovery-provider](https://github.com/OmniTrustILM/ct-logs-discovery-provider)         | Discovery provider for Certificate Transparency logs          |
| [keystore-entity-provider](https://github.com/OmniTrustILM/keystore-entity-provider)             | Entity provider for managing certificates in Java Keystores   |
| [software-cryptography-provider](https://github.com/OmniTrustILM/software-cryptography-provider) | Cryptography provider for managing keys in software keystores |
| [email-notification-provider](https://github.com/OmniTrustILM/email-notification-provider)       | Email notification provider                                   |
| [webhook-notification-provider](https://github.com/OmniTrustILM/webhook-notification-provider)   | Webhook notification provider                                 |

### Integrations

| Repository                                                                 | Description                                   |
|----------------------------------------------------------------------------|-----------------------------------------------|
| [cert-manager-issuer](https://github.com/OmniTrustILM/cert-manager-issuer) | cert-manager external issuer for Kubernetes   |
| [csc-api](https://github.com/OmniTrustILM/csc-api)                         | Cloud Signature Consortium API implementation |
| [mcp-server](https://github.com/OmniTrustILM/mcp-server)                   | ILM MCP Server                                |
| [go-sdk](https://github.com/OmniTrustILM/go-sdk)                           | Go SDK for ILM platform                       |

### Deployment and Operations

| Repository                                                                     | Description                             |
|--------------------------------------------------------------------------------|-----------------------------------------|
| [helm-charts](https://github.com/OmniTrustILM/helm-charts)                     | Helm charts to install and maintain ILM |
| [appliance](https://github.com/OmniTrustILM/appliance)                         | ILM virtual appliance                   |
| [appliance-tools](https://github.com/OmniTrustILM/appliance-tools)             | Debian package with ILM appliance tools |
| [keycloak-theme](https://github.com/OmniTrustILM/keycloak-theme)               | ILM custom Keycloak theme               |
| [keycloak-optimized](https://github.com/OmniTrustILM/keycloak-optimized)       | Optimized Keycloak docker image         |
| [provisioning-rabbitmq](https://github.com/OmniTrustILM/provisioning-rabbitmq) | Provisioning service for RabbitMQ       |

### Documentation

| Repository                                                                         | Description                                            |
|------------------------------------------------------------------------------------|--------------------------------------------------------|
| [documentation](https://github.com/OmniTrustILM/documentation)                     | Platform documentation for contributors and developers |
| [interface-documentation](https://github.com/OmniTrustILM/interface-documentation) | Interface and API documentation                        |

## Contribution

Anyone can contribute to ILM and we would be happy to support you in that. See [Contribution Guide](CONTRIBUTING.md) for more information.

## License

The ILM platform is released under the [MIT License](LICENSE.md). Some connectors and user interfaces are released under their own licenses or subscriptions. Consult with us for more information.
