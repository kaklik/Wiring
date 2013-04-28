About Wiring
============

Wiring is an open-source programming framework for microcontrollers.

Wiring allows writing cross-platform software to control devices
attached to a wide range of microcontroller boards to create all kinds
of creative coding, interactive objects, spaces or physical experiences.
The framework is thoughtfully created with designers and artists in 
mind to encourage a community where beginners through experts from 
around the world share ideas, knowledge and their collective experience.
There are thousands of students, artists, designers, researchers, and
hobbyists who use Wiring for learning, prototyping, and finished
professional work production. 

Wiring's Components
===================

Wiring has three major components:

* The Wiring Language: A thin layer on top of C++ which simplifies the
  process of writing embedded programs.

* The Wiring Framework: A C and C++ API for writing embedded programs,
  either using C++ or the Wiring Language. Currently, a implementation
  of the Wiring framework exists for 8-bit AVR
  microcontrollers. Support for the STM32 line of ARM Cortex M3 and M4
  microcontrollers is in progress.

* Wiring IDE: A cross-platform Integrated Development Environment
  (IDE) used to write, compile, and upload programs written in the
  Wiring language to boards which support the Wiring Framework.

This source code repository contains the Wiring Framework and the
Wiring IDE.

Getting Wiring
==============

This is the source code repository for the Wiring IDE and Wiring
Framework. If you just want to write and upload programs, your best
bet is to download an existing binary release. These are available at
the Wiring web site for Windows, Mac, and Linux:

   http://wiring.org.co/download/

If you are interested in developing Wiring, you'll need to build the
IDE using this repository.  For more information, see the file
build/howto.txt (in this repository).

Developing Wiring
=================

Development discussion takes place on
wiring-dev@yahoogroups.ca. Please ask any development-related
questions there. To subscribe, send email to:

  wiring-dev-subscribe@yahoogroups.ca.

Archives are available online at:

  http://ca.groups.yahoo.com/group/wiring-dev/

The developers' portal on the Wiring Wiki is here:

  http://wiki.wiring.co/wiki/Develop_Wiring

Repository Structure
====================

The Wiring repository structure is as follows:

* IDE/: Contains the Java sources for the Wiring IDE. The main entry
  point is in IDE/processing/app/Base.java.

* framework/: Contains the Wiring Framework, associated libraries, and
  its implementations. These implementations (called "cores") contain
  the nonportable code which targets a concrete microcontroller (or
  family of microcontrollers).

* build: Files used when building the Wiring IDE.

* out/: [generated] This directory is autogenerated during the build
  process. It contains all of the build artifacts. After a build, this
  directory includes any downloaded dependencies, Java class and jar
  files, and the distributable IDE bundles.
