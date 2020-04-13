# Gradle Build Templates

Provides quick bootstrap scripts for spring-boot, spring-modules/jar which includes common plugins/capabilities used across microservices.
Versions can be managed by the services which imports the scripts. Additional configurations for the plugins can be applied by the DSL related to the plugins.

## How to use the common scripts

Add the following snippet to `build.gradle` to include build script configuration - TBD (move to plugin management)
```
buildscript { 
	apply from: "https://raw.githubusercontent.com/dheeraj-mummareddy/gradle-build-templates/master/gradle-common/init-buildscript.gradle", to: buildscript
}
```

### Spring boot
Enable spring boot bootstrap configurations by applying configuration
```
apply from: 'https://raw.githubusercontent.com/dheeraj-mummareddy/gradle-build-templates/master/spring-boot/spring-rest-jumpstart.gradle'
```

### Spring JAR
Enable spring jar bootstrap configurations by applying configuration
```
apply from: 'https://raw.githubusercontent.com/dheeraj-mummareddy/gradle-build-templates/master/spring-library/spring-jar-jumpstart.gradle'
```


## Versioning

TDB

## JDK Support

TBD - abstract out the jdk support

## Supported common plugins

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

## Support highlevel common scripts/tasks

- code quality
- docker
- packaging
- datadog
- integration tests
- performance tests
- semantic release

## Configurable gradle properties

| Property Name                         | Dependency/Plugin     | Default                   |
|---------------------------------------|-----------------------|---------------------------|
| `localSpringProfile`                  | Spring                | local                     |
| `gradleTemplatesSource`               | gradle                |                           |
| `codeQualityResources`                | plugins               |                           |
| `integrationTestSpringProfile`        | spring                | integrationTest           |
| `integrationTestSourceRoot`           | gradle                | src/integration-test      |
| `performanceTestSourceRoot`           | gradle                | src/perf-test             |
| `sonarOrganization`                   | sonar                 |                           |
| `sonarHostUrl`                        | sonar                 | https://sonarcloud.io   	|

| Property Name                         | Dependency/Plugin     | Default                   |
|---------------------------------------|-----------------------|---------------------------|
| `springCloudVersion`                  | Spring                | Hoxton.SR3	            |
| `scalaVersion`                        | scala                 | 2.13.1                    |
| `gatlingVersion`                      | gatling               | 3.3.1                     |
| `checkStyleVersion`                   | checkstyle            | 8.17                      |
| `pmdVersion`                          | pmd                   | 6.21.0                    |
| `jacocoVersion`                       | jacoco                | 0.8.5                     |
| `spotBugsVersion`                     | spotBugs              | 3.1.11                    |
| `objenesisVersion`                    | objenesis             | 3.1                       |
| `hamcrestAllVersion`                  | hamcrest              | 1.3                       |
| `assertJVersion`                      | assert                | 3.14.0                    |
| `junitToolBoxVersion`                 | junit                 | 2.4                       |
| `junitJupiterTestcontainersVersion`   | junit                 | 1.13.0                    |
| `datadogAgentVersion`                 | datadog               | 0.47.0                    |


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

- Spring boot

## Spring jar gradle bootstrap

Provides quick bootstrap scripts for a spring library which helps building, packaging and containerzing spring library projects.

* Supported plugins

- Java jar

### semantic versioning stretergy
TBD

### Example Projects
CI - TBD