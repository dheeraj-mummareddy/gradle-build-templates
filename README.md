# Gradle Build Templates

Provides quick bootstrap scripts for spring-boot, spring-modules/jar which includes common plugins/capabilities used across microservices.
All the version are managed by the services which imports the scripts. 

* Supported common plugins

- java
- groovy
- scala
- idea
- maven
- gradle-lombok
- sonarqube
- scala
- checkstyle
- pmd
- jacoco
- spotbugs
- lombok

* Support highlevel common scripts/tasks

- code quality
- docker
- packaging
- datadog
- integration tests
- performance tests
- semantic release

* Required/Optional gradle properties - TDB

TBD - move plugin configuration from build script to plugin management and externalize plugin version properties.

| Property Name                         | Dependency/Plugin     |
|---------------------------------------|-----------------------|
| `description`                         | Spring boot/project   |
| `lombokPluginVersion`                 | Lombok                |
| `spotbugsPluginVersion`               | Sonarqube             |
| `sonarqubePluginVersion`              | Sonarqube             |
| `springBootPluginVersion`             | Spring Boot           |
| `springDependencyMgntPluginVersion`   | Spring Dependencies   |



## Spring boot gradle bootstrap

Provides quick bootstrap scripts for spring-boot which helps building, packaging and containerzing spring boot projects.

* Supported plugins

- spring boot

### version properties with defaults

`datadogAgentVersion`


### semantic versioning stretergy
TBD

