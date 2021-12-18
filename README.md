# SolarSystemAR

1. General Structure of Application:\

  1.1. General Structure of Folders:\
  I have grouped my application files structured inside the DataFiles folder.\ 
  I have Animations, Audios, Fonts, Logo, Materials, Scenes, Scripts, and Textures folder in the DataFiles folder. 
  I also structured each of these subfolders according to my scenes. 
  For example, I have three scenes in my application which are named as MenuScene, ARScene, InformationScene 
  thus I have ARSceneTextures, InformationSceneTextures, and MenuSceneTextures folders inside the Textures folder. 
  
  1.2. General Structure of Scripts:
  I have ButtonStates folder which holds the information about the buttons on InformationScene, 
  HandlingPlanetInformations folder which holds the content of the planets in InformationScene, 
  ChangingButtonImageDynamically.cs file which changes the PlanetButton image in ARScene when the target image is found, 
  HandlingButtonEvents.cs file which redirects application between scenes, PlanetRing.cs file which creates a ring for Saturn, 
  Rotation.cs file which rotates planets around their center.

2. Description of Application:
  First I created the MenuScene. MenuScene has Start and Exit buttons. 
  When the start button is pressed, it goes to ARScene where image targets are recognized, 
  and when the exit button is pressed, the application exits. 
  
  Secondly, I created the ARScene. Since I use the Marker-Based Augmented Reality approach in my application, 
  I have imported the Vuforia package into my application for the recognition of image targets. 
  Then I used an AR Camera instead of the Main Camera. I put Image Targets in Vuforia's database 
  and imported the database into my application. Then I used these image targets in my application. 
  I placed planets on these image targets. I created three buttons on the left side of the screen in ARScene. 
  When the home page button is pressed, the application is directed to the MenuScene, which is opened at first. 
  When the Exit button is pressed, the application is terminated. When the Planet button is pressed, 
  the planet information is transferred to the InformationScene according to the image target 
  and the application is directed to the InformationScene, which contains the information of the planets. 
  At the same time, the background image of the Planet button changes dynamically according to the planet recognized by the camera. 

  Finally, I created the InformationScene. General information about the planets is shown here. 
  There are five buttons in the InformationScene. When the Back button is pressed, the application is directed to ARScene. 
  When the location information button is pressed, the planet's distance from the sun is displayed on the screen. 
  When the Other informations button is pressed, detailed information about the planet is displayed on the screen. 
  When the Left button is pressed, it switches between the other information pages to the left. 
  When the Right button is pressed, it switches between the other information pages to the right. 
  
WARNING!!!
  After I finished my Unity application, I built this Unity project for the application to work on Android devices. 
  In order for the mobile application to work on the Android platform, the Android version must be at least Android 6.0 (Marshmallow).
