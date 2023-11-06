Developing Drools and jBPM
==========================

**If you want to build or contribute to a kiegroup project, [read this document](https://github.com/kiegroup/droolsjbpm-build-bootstrap/blob/master/README.md).**

**It will save you and us a lot of time by setting up your development environment correctly.**
It solves all known pitfalls that can disrupt your development.
It also describes all guidelines, tips and tricks.
If you want your pull requests (or patches) to be merged, please respect those guidelines.

## How to build KIE Server?

1. Go to the `kie-server-parent` folder

2. Run the following command in the project's root path.
<br>`mvn clean install -e -U -DskipTests`

3. Once the building is completed, go to
<br>`kie-server-parent -> kie-server-wars -> kie-server -> target -> kie-server-7.74.0-SNAPSHOT-ee8.war`

4. Rename `kie-server-7.74.0-SNAPSHOT-ee8.war` as `kie-server.war`

5. Go to the folder and replace `kie-server.war`
<br>`standalone -> deployments -> kie-server.war`
