---
permalink: /dev/
title: "Source & Documentation"
classes: wide2
header:
  overlay_color: "#000"
  overlay_filter: "0.4"
  overlay_image: /assets/images/dev.jpeg
  caption: "Photo credit: [**Fotis Fotopoulos**](https://unsplash.com/photos/DuHKoV44prg)"
  actions:
    - label: "Github"
      url: "https://github.com/libgdx/libgdx"
    - label: "Issue Tracker"
      url: "https://github.com/libgdx/libgdx/issues"
    - label: "Wiki"
      url: "https://github.com/libgdx/libgdx/wiki"

excerpt: "LibGDX is hosted on Github, where all team members collaborate. Fork, star and contribute to our project!."


toc: true
toc_sticky: false # =not on top
#header:
#  overlay_image: /assets/images/unsplash-image-1.jpg
#  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
#  actions:
#    - label: "Link to somewhere"
#      url: "https://github.com"
---

# How to get started with libGDX?
## Set up a new project
LibGDX offers a community-made setup tool, which automatically creates a project and downloads everything necessary. You can download the setup tool [here](https://github.com/tommyettinger/gdx-liftoff/releases). Setup instruction can be found [here](/dev/setup/). See [here](/dev/running/) on how to get an imported project running.

## First Game
Our [wiki](https://github.com/libgdx/libgdx/wiki/A-Simple-Game) details how you can create your very first libGDX game. If you're new to game dev and have never developed a game before, take a look at this (even more straight-forward) [tutorial](http://tann.space/HelloLibgdx/) by tann.

<br/>

# Documentation
The libGDX codebase is documented in two ways:
- In our [Wiki](https://github.com/libgdx/libgdx/wiki)
- And via the [Javadoc](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/)

<br/>

# Tools & Frameworks
## Tools
There are different tools that make the development process for libGDX easier. See [here](/dev/tools/) for a collection.

## Frameworks
A curated list of our favourite frameworks can be found [here](https://github.com/rafaskb/awesome-libgdx). On our Discord server we also have an extensive collection of libGDX-centered frameworks that are currently work in progress.

<br/>

# Contributing to libGDX
Contributing to LibGDX can come in a few different forms, you can help out on our discord, pledge to the [patreon page](https://www.patreon.com/libgdx), or submit code and [documentation](https://github.com/libgdx/libgdx/wiki) back to the project on github.

## Reporting an Issue
Please note the issue tracker isn't for personal assistance, if you have a problem that isn't a reproducable bug in the core framework, please use the [community](/community/) for assistance.
{: .notice--primary}

Before you report the issue on our issue tracker we ask you to do a few things:
- Verify that the task hasn't already been reported on the tracker
- Make sure the bug hasn't already been fixed, use the latest SNAPSHOT of LibGDX to latest
- Create a self contained example to demonstrate the issue. Don't hack a project down, start fresh to reproduce the error.

Once you have done this, please submit this along with any stacktraces or assets to the [issue tracker](https://github.com/libgdx/libgdx/issues), whilst filling out the template that is shown when creating a new issue.

## Working from Source
If you want to contribute to libGDX itself, you need to get it set up on your local machine. For this, Android Studio is strongly recommended as IDE!

If you want to submit code back to the project, please take a moment to review our [guidelines](/dev/contributing/).

### Set Up
1. Fork libGDX and clone the repo:
```
git clone git://github.com/libgdx/libgdx.git
cd libgdx
```
2. Fetch the native binaries, which were built on the snapshot build server. Even if you plan on building natives later yourself, it's recommended to bring these down so you can test your development environment is setup correctly before moving to the next step.
```
./gradlew fetchNatives
```
3. Importing the project:

  a) Via IntelliJ/Android Studio:
     - File > Open > LibGDX root build.gradle
     - Import all projects
     - Wait until everything is synced and indexed
     - View > Tool Windows > Gradle, sync gradle button
     - Make sure the Gradle sync succeeds, if not resolve the issues at hand.
     - Go into preferences and turn off configure on demand
     - Try running the LwjglTestStart class located in tests/gdx-tests/gdx-tests-lwjgl/src by right clicking and running
     - You should get assets not found when you try to run a test, edit the run configuration and point it to the correct assets folder (tests/gdx-tests-android/assets)

![](/assets/images/dev/source/0.png)

  b) Via Eclipse: File > Import > Gradle > Gradle project

### Building
All of the other projects are hooked up and ready to test given that you have set up your system correctly, so give them a go.

Its recommended to run the android and gwt tests on command line with the following:

```
./gradlew tests:gdx-tests-android:installDebug

./gradlew tests:gdx-tests-gwt:superDev
```

To use your local changes in another project, you can install libGDX to your local maven repository by running the following command:
```
mvn install
```

This will build and install LibGDX and all core components to your local maven repository with the current version declared in the pom.xml files.

### Natives
If you want to build the libGDX natives yourself, you can find [instructions](/dev/natives/) here.
