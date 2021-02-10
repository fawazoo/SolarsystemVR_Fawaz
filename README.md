# SolarsystemVR_Fawaz

## FAWAZ_NADEEM, MS CSE20, RCMS ,REG#00000328009, PROJECT_2_VR

###Summary

Solarsystem was designed for a VR Google cardboard mobile Application using unity.
Basically an educative demo aimed for primary students. 
The aim is create an interactive environment for students by introducing technological developement for a vivid experience.
Using this app gives an environemnt to explore space in a 3d virtual reality. The position of camera is placed such that the planets can be viewed at 20-30 degree angle up, with the sun directly above the viewer to give a feel of exploration with a 360 degree view from all sides. With audio running on the back and planet information provided on gaze interation and tranformation of planet objects proviing factual info of how planet rotation works. 

####Steps

Basic step starts from installing unity from website. Free version available for those not earning minimum requirement mentioned on website.
On Unity hub, Download the version suitable with add ons that is required i.e. in this case, android environment with ndk package.
Open up a new 3d project. Place objects, camera etc on the heirachy to be viewed in the scene area. You can edit them from inspector.
Transfer necessary files (textures, materials, scripts) that can be used for transformations, color editing etc for your Vr environamnet designinig.
In our case, create 3d spheres, transform them for solar system designing, add textures, sound effects.
Add scripts to produce unique transformations such as rotation.
Download the googlecardboard package (GoogleVRForUnity-1.190.1) from github and import. From this, we select the emulators for the environment of google cardboard. Add GvrEventSystem, GvrEditorEmulator to sample scene. Add GvrReticlePointer under camera and a Raycaster script.

####Steps to create apk file:

We start by downloading ndk and VR support sdk files:
-> android.sdk
->android-ndk-r16b
make sure these two files are runnning from preferences.
Go to build settings and switch build to android. Also add the scene.
Check player settings and other options. change package name to com.RCMSVR.Your_name.
Keep minimum level api android apk 16 till automatic highest required.
In xr settings, select Vr cardboard.
Once all this is done, we can build our apk file from build settings and our VR App is ready to go.

#####Issues Faced:
Downloading the 2020 version of unity, Building the apk was a problem caused by the bug from unty.
The ndk package was not getting downloaded for android package from hub.
Using the 2019 version also created an issue for having multiple OS files in its library. 
Issue still remained unresolved.
2018 version worked well but sdk file had to be downloaded from android studio.


