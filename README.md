# JDemetra+ archetypes
[Maven templates](https://maven.apache.org/guides/introduction/introduction-to-archetypes.html) for [JDemetra+](https://github.com/jdemetra/jdemetra-app).  

Available templates:

| ArtifactId | Description |
| ---------- | ----------- |
| `demetra-archetype-quickstart` | An archetype to generate an empty skeleton of a JDemetra+ extension |

## Pre-requisites
- JDK 1.7 or later
- maven 3.0 or later

## How to use in NetBeans

1. Open the wizard by clicking on `File > New Project...` menu.

2. In step 1, choose `Maven > Project from Archetype`.

3. In step 2, put the following properties:  

| Key | Value |
| --- | ----- |
| Group ID | `be.nbb.demetra` |
| Artifact ID | `demetra-archetype-quickstart` |
| Version | `2.1.0-SNAPSHOT` |
| Repository | `https://oss.jfrog.org/artifactory/oss-snapshot-local` |

4. In step 3, fill the required properties.

5. Click on `finish` to generate the project.

## How to use in command line

Open a terminal and copy/paste:

```Shell
mvn archetype:generate -DarchetypeRepository=https://oss.jfrog.org/artifactory/oss-snapshot-local -DarchetypeGroupId=be.nbb.demetra -DarchetypeArtifactId=demetra-archetype-quickstart -DarchetypeVersion=2.1.0-SNAPSHOT
```

Fill in the required properties and proceed.

Then cd into the generated project; you can build it like any other Maven project.

## How to build the archetype

If you have Maven and Git installed, simply issue the following commands in a terminal to clone this GitHub repository and build the archetype with Maven:

```Shell
git clone git://github.com/nbbrd/jdemetra-archetypes.git
cd jdemetra-archetypes
mvn install
```
