# MySparkArchetype
# Spark Archetype for Maven
This Archetype helps people interested in trying spark for the first to get a working demo up in seconds.

## Build and Install the Archetype

mvn install

This will compile the Archetype sources and install them into your local maven repository.

##Generate the Hello World Spark Project from the Archetype
Navigate to the directory where the new program will be created and run the following maven command:

mvn archetype:generate \
-DarchetypeGroupId=us.mohindra \
-DarchetypeArtifactId=spark-1.2-archetype \
-DarchetypeVersion=1.0-SNAPSHOT \
-DgroupId=your.groupid.here \
-DartifactId=your-artifactid-here \
-Dversion=1.0-SNAPSHOT \
-Dpackage=us.mohindra


IF YOU ARE USING ECLIPSE change pom.xml in the generated project 

FROM

<build>
<sourceDirectory>src/main</sourceDirectory>
<testSourceDirectory>src/test</testSourceDirectory>
...

TO

<build>
<sourceDirectory>src/main/java</sourceDirectory>
<testSourceDirectory>src/test/java</testSourceDirectory>
...