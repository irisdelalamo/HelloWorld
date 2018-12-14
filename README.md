# Dead simple, boiler plate getting started Java app with maven
Skeleton Java project with a vanilla maven file with minimal options to get you started.

#### Notes ####
This project contains a gitignore that will stop most IDE specific files as well as Java build files from being checked into source control. It's generally good practice to only contain core files that are needed for the project to run. Since Maven, Gradle, or Ant (not really anymore) control the build process and project attributes we don't need to hold on to project specific files from IDEA, NetBeans, Eclipse, etc.

#### Getting started example with IDEA ####

##### Build project to a *.jar #####
* Git clone this project to your local workstation.
* Open IntelliJ IDEA and select the option to import an project
* After going through the import process we will open the File menu and select Project Structure.
* Select the Artifacts tab
* Click the plus (+) sign and add JAR -> Empty.
* Make sure your output directory at the top is desireable. I usually select bin/ to put the jar
* Select "Build on Make" checkbox
* Make sure the manifest is selected
* Right-click your *.jar inside output layout. Select Add a Copy of -> Module Output
