# Athena Parent

## Purpose
This module contains the über POM for all Athena projects. It defines the Java and Maven plugin versions that are 
being used throughout all projects. It also includes AssertJ, Mockito and Lombok.

The POM includes two profiles: **qa** and **release**.

- **qa**. This profile performs OWASP dependency checks to detect vulnerabilities, JaCoCo code coverage and a 
SonarQube code quality scan.


- **release**. This profile adds the generation of sources and javadoc archives that can be uploaded to repositories.

Both profiles have to be applied when a project is released, and therefore should be part of any release pipeline.