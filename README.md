Android-Project-Manager
=======================

Allows for easier management of android projects from command line.

When writing Android applications, I tend not to like using eclipse.  And this python script was
created to address that.  Instead of having to remember all the commands, I have bundled the most
important ones to me here.

Dependencies
------------
* Python 3
* Android sdk
* Ant

Usage
-----

To use you must place the Android sdk in your home folder.  Next you must rename the folder to .android.  Make sure to add
platform-tools and tools to your path.  Once this is done, there are three commands that are available to you.  Please
note that the build and install command assume that you are running the script in the project's root directory.

* Create
* Build
* Install
* Help

###Create
This command will prompt for the project name, a package name, and the target sdk version.  This script assumes
that you have at least one sdk version installed, and package names must follow Java's package name rules.
When creating your project it will first create a folder with the same name as your project in your current directory,
and it will create the necessary files using the android command.

###Build
Builds your project using ant.

###Install
I find emulators very slow.  Because of this the install command only installs the apk to a phone that is connected
to your computer.

###Help
Displays a brief help document, with the commands and their usage.
