---
permalink: /dev/running/
title: "Running a Project"
classes: wide2
header:
  overlay_color: "#000"
  overlay_filter: "0.3"
  overlay_image: /assets/images/dev/dev.jpeg
  caption: "Photo credit: [**Florian Olivo**](https://unsplash.com/photos/Ek9Znm8lQ1U)"

toc: true
toc_sticky: false # =not on top

---

{% include breadcrumbs.html %}

This article explains how you can get your imported projects running.

# Desktop
## IDEA/Android Studio:
1. Right click your DesktopLauncher class
2. Select 'Run DesktopLauncher.main()'. This should fail with missing assets, because we need to hook up the assets folder first.
3. Open up Run Configurations

![](/assets/images/dev/idea/0.png)

4. Edit the Run Configuration that was just created by running the desktop project and set the working directory to point to your `core/assets` folder

![](/assets/images/dev/idea/1.png)

5. Run your application using the run button

## Eclipse:
1. Right click your desktop project > Build Path > Configure Build Path
2. Click the sources tab, and click 'Add Folder'
3. Select the assets folder and hit OK.

![](/assets/images/dev/eclipse/0.png)

4. Right click your desktop project > Run as > Java Application

## Netbeans:
Right click the desktop project > Run

<br/>

# Android
- **IDEA/Android Studio:** Right click AndroidLauncher > Run AndroidLauncher
- **Eclipse:** Right click Android project > Run As > AndroidApplication
- **Netbeans:** Right click Android project > Run As > AndroidApplication

<br/>

# iOS
## IDEA/Android Studio
1. Open Run/Debug Configurations
2. Create a new run configuration for a RoboVM iOS application

![](/assets/images/dev/idea/2.png)

3. Select the provisioning profile and simulator/device target
4. Run the created run configuration

For more information on using and configuring the RoboVM intellij plugin please see the [documentation](http://robovm.mobidevelop.com).

NOTE: The documentation is for the 'Official' RoboVM plugin, we currently use a fork of this. <br/> <br/> This means some of the information (such as license information) is redundant, however configuring and using the plugin should be very similar.
{: .notice--primary}

## Eclipse
- Right click the iOS RoboVM project > Run As > RoboVM runner of your choice

![](/assets/images/dev/eclipse/1.png)

For more information on using and configuring the RoboVM intellij plugin please see the [documentation](http://robovm.mobidevelop.com).

NOTE: The documentation is for the 'Official' RoboVM plugin, we currently use a fork of this. <br/> <br/> This means some of the information (such as license information) is redundant, however configuring and using the plugin should be very similar.
{: .notice--primary}

<br/>

# HTML
HTML is best suited to be run on command line. You are welcome to manually setup GWT in the IDE of your choice if you are familiar with it, but the recommended way is to drop down to terminal or command prompt.

The HTML target can be run in **Super Dev** mode, which allows you to recompile on the fly, and debug your application in browser.

To do so, open up your favourite shell or terminal, change directory to the project directory and invoke the respective gradle task:

```
./gradlew html:superDev
```

**On Unix:** If you get a permission denied error, set the execution flag on the gradlew file: `chmod +x gradlew`
{: .notice--primary}

You should see lots of text wizzing by, and if all goes well you should see the following line at the end:

![](/assets/images/dev/html/0.png)

You can then go to [`http://localhost:8080/index.html`](http://localhost:8080/index.html), to see your application running, with a recompile button.

For further info on configuring and debugging with SuperDev check the [GWT documentation](http://www.gwtproject.org/articles/superdevmode.html).

<br/>

# Command Line
All the targets can be run and deployed to via the command line interface.

**Desktop:**
```
./gradlew desktop:run
```

**Android:**
```
./gradlew android:installDebug android:run
```

**iOS:**
```
./gradlew ios:launchIPhoneSimulator
```

**HTML:**
```
./gradlew html:superDev
```

<br/>

# What to do next?
Now that you're done with the set up, you can get to do some real coding. See [here](/dev/) for some pointers on where to start.
