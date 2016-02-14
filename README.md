
# Synesthesia

This Android App simulates Grapheme Color Synesthesia.  People with this rare
ability see letters and numbers in different colors, even though the letters
in the text they are reading is only a single color (typically black).

People with synesthesia frequently test better on memory for text and
numbers than people without it.  There are other kinds of synesthesia,
and a number of well-known artists and scientists claim it important
to their achievements.   You can read up on it on Wikipedia.


Using the app is simple.  Just point the rectangualr box at the top of the
screen at some text, hold still, and the letters in the text will appear
lower on the screen in full color.


## Future Development

I'm developing this App as part of a series of experiments with Augmented
Reality.  The intent is to build an app that simulates synesthesia as
faithfully as possible in a 3d heads-up display.  I'm starting on Android
phones because that's what I have, that's where my career is headed and
many AR HMDs available or in development are Android-based.

Plans for the app are outlined here:

[Enhancements](https://github.com/fermigas/Synesthesia/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement)

See this issue, in particular:  [Overlay Mode.](https://github.com/fermigas/Synesthesia/issues/4)

Note that there's no time-frame for when these will be added.

## Known Issues

Known issues/bugs are tracked [here](https://github.com/fermigas/Synesthesia/issues?q=is%3Aissue+is%3Aopen+label%3Abug)

Feel free to contribute with a pull request.

## Building Synesthesia

This app uses the Vuforia Augmented Reality SDK and the code is a heavily-
hacked version of one of their samples.

###  How To Register as a Vuforia Developer

You'll need to register in order to get the SDK and samples.  While not
strictly necessary as everything in this app is self-contained, you will
neer to register in order to get a license key (see below).

Register [here](http://developer.vuforia.com/library/articles/Solution/How-To-Register-as-a-Vuforia-Developer)

### How to Create A License Key

Instructions [here](http://developer.vuforia.com/library/articles/Solution/How-To-Create-an-App-License)

### Getting a License Key
Get your license [here] (https://developer.vuforia.com/targetmanager/licenseManager/licenseListing)

### Using the License Key in your App

Next, add  your Vuforia License Key to the code by adding the following to your
~/.gradle/gradle.properties file:

VuforiaLicenseKey="[Your Vuforia License Key]"

In your build.gradle  (Module: app) these lines will reference the key:

buildTypes.each{
     it.buildConfigField 'String', 'VUFORIA_LICENSE_KEY', VuforiaLicenseKey
}


### Get the SDK and Samples Here
Vuforia Downloads [page](https://developer.vuforia.com/downloads/sdk)







