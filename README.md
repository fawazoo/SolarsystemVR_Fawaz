# SolarsystemVR_Fawaz

## FAWAZ_NADEEM, MS CSE20, RCMS ,REG#00000328009, PROJECT_2_VR

###Summary

Solarsystem was designed for a VR Google cardboard mobile Application using unity.
Basically an educative demo aimed for primary students. 
The aim is to create an interactive environment for students by introducing technological developement for a vivid experience.
Using this app gives an environemnt to explore space in a 3d virtual reality. The position of camera is placed such that the planets can be viewed at 10-30 degree angle up, with the sun directly above the viewer to give a feel of exploration with a 360 degree view from all sides. With audio running on the back and planet information provided on gaze interation and tranformation of planet objects proviing physical info of how planet rotation works. The use of textures similar to real planets and planetary roation gives the imersive feeling.

####Steps

Basic step starts from installing unity from website. Free version available for those not earning minimum requirement mentioned on website.
On Unity hub, Download the version suitable with add ons that is required i.e. in this case, android environment with ndk package.
Open up a new 3d project. Place objects, camera etc on the heirachy to be viewed in the scene area. You can edit them from inspector.
Transfer necessary files (textures, materials, scripts) that can be used for transformations, color editing etc for your Vr environamnet designinig.
In our case, create 3d spheres, transform them for solar system designing, add textures, sound effects.
Add scripts to produce unique transformations. Rotation used for solar syatem movement of the planets with respect to itself and the sun.
The image viewer script was used to enable information window to pop up while gazing onto a planet.
Add textures to each planet and check the emission so that the texture of each planet can be viewed. 
We also add an additional point light inside the sun to give the experience of sun emitting light giving shadows on the planets. This shows how for example on earth, night and day happens with rotations.
6 sided space material is added into the skybox to create the 'space'
Download the googlecardboard package (GoogleVRForUnity-1.190.1) from github and import. From this, we select the emulators for the environment of google cardboard. Add GvrEventSystem, GvrEditorEmulator to sample scene. Add GvrReticlePointer under camera and a Raycaster script(enabling for use of googlevr). 
Add the pointerphysicsraycaster on the camera to show a pointer for gaze interations.
Add sounds onto objects(planets) the buring sound was added to the sun while the space sound added into the space.
Convert the images and add to canvas. Add image script file to objects and place the info images. Add event trigger pointer enter and exit.

####Steps to create apk file:

We start by downloading ndk and VR support sdk files:
-> android.sdk
->android-ndk-r16b
Make sure these two files are runnning from preferences.
Go to build settings and switch build to Android and add scene.
Then go to player seetings<other settings.
Change package name to com.RCMSVR.Your_name.
Keep minimum level api android apk 20-24 till automatic highest required.
In xr settings, select Vr cardboard.
Once all this is done, we can build our apk file from build settings and our VR App is ready to go.

#####Issues Faced:
Downloading the 2020 version of unity, Building the apk was a problem caused by the bug from unty.
The ndk package was not getting downloaded for android package from hub.
Using the 2019 version also created an issue for having multiple OS files in its library. 
Issue still remained unresolved.
2018 version worked well but sdk file had to be downloaded from android studio.
Script writing also was a problem. Using visual studio for sdk purpose made problems as unity did not recognize the script file.
Script file required 'monobehaviour' that was not being recognized. One resolution was to name both script file and defined in program same.
Applying image viewing script was problematic. Gazing at planets at particular times while play casued image to glitch multiple times unitl it fixes itself. It can be resolved if the planets were placed far and away from each other.
Another problem arised was the pointer raycaster. It cannot identify far away objetcs. limited range was only availbe to target close planets. It is difficult to place pluto in range that can cause the solar rotation view inadequate. 
We cannot put planets close in range, resulting in poor qulaity environment. Changing position of camera would remove the emersive quality from the Googlevr environment.

#####Remarks
Many more implemetations can be made. With time, solar sysatm can also be placed in the actual environment, depiction AR which would not required google cardboard. Much more better VR systems of interations have been made that can enhance the quality and more movement other then the head. More improvements can be made in this project with more practice and learning new techniques.


