<p align="center">
  <img src="https://avatars.githubusercontent.com/u/55738436?s=400&u=94e444521358ab1d18ef15de2df480bac1177abe&v=4" alt="SE Spaceship Logo" width="200"/>
</p>

<p align="center">
  <a href="https://github.com/boriszbandi/se-lab/actions/workflows/maven.yml">
    <img src="https://github.com/boriszbandi/se-lab/actions/workflows/maven.yml/badge.svg" alt="Maven Build"/>
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT"/>
  </a>
</p>

<h1 align="center">SE Spaceship</h1>

<p align="center">
  This is a sample application for the <a href="http://www.mit.bme.hu/oktatas/targyak/vimiab04">Software Engineering</a> course at BME MIT.
  The application is simplified and deliberately contains bugs.
</p>

## Getting Started

- The project is implemented in Java 11.
- The project can be built using [Maven](https://maven.apache.org/).
- [JUnit](https://junit.org/junit5/) is used for tests, and [Mockito](https://site.mockito.org/) for isolating dependencies.

### Build the Application

Clone the repository and execute Maven to build the application:


```
mvn compile
```

To compile and run tests also execute:

```
mvn test
```

(That will be enough to know for the current exercises. If you are more interested, see [this](https://github.com/ftsrg-edu/swsv-labs/wiki/0b-Build-tools) short guide about Maven.)

As this is a really simple project, you can use the command-line build tools or a light-weight IDE like [Visual Studio Code](https://code.visualstudio.com/).

## Overview

The project represents an alpha version of a spaceship.

- The ship (`SpaceShip` interface) can fire one or more lasers or torpedos.
- We have only one spaceship as of now (`GT4500`).
- Currently two firing modes (`FiringMode`) are supported: firing only one or all instances of a given weapon type.
- Lasers are not yet implemented, but the code for torpedo stores are ready (`TorpedoStore`).
- For the GT4500 ship the rules for firing torpedoes can be found in the Javadoc comment of method `fireTorpedos`. They are already partially implemented.
- There are currently two tests (`GT4500Test`), but be aware that they are not proper unit tests, as they do not isolate the dependencies of the tested class.

The code can be built, but due to missing features one of the tests fails. The first exercise will be to fix this.


