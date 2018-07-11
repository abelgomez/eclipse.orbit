# Abel Gómez's (kind of) Orbit Repository

This repository provides bundles containing 3rd party libraries not available in the official Eclipse Orbit repository (http://download.eclipse.org/tools/orbit/downloads/) and used in many of my Eclipse-based projects.

## Warning! Warning! Warning!

For convenience purposes, some of the bundles contained in this repository contain all their transitive dependencies (e.g., HBase).
While this is fine when using the bundles in Eclipse/OSGi-based environments, this may be a source of problems (a.k.k. [JAR Hell](https://en.wikipedia.org/wiki/Java_Classloader#JAR_hell)) when the bundles are used in unplanned ways (e.g., extracting the bundle contents and blindly adding the packaged JARs to the classpath of a regular Java application).
Such problems may happen unnoticeably, and in case they are detected, they may be hard to chase and fix.
**You've been warned :)**

## Licensing

Manifest files included in the `master` branch of this repository are freely provided to the public domain. 

3rd party JAR library files have their own licenses. Please check the `feature.xml` manifest files in the corresponding [feature definitions](features/).
