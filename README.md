# SolarSystemAR

A. General Structure of Application:  

&nbsp;&nbsp;A.1. General Structure of Folders:  
&nbsp;&nbsp;I have grouped my application files structured inside the DataFiles folder.  
&nbsp;&nbsp;I have Animations, Audios, Fonts, Logo, Materials, Scenes, Scripts, and Textures folder in the DataFiles folder.  
&nbsp;&nbsp;I also structured each of these subfolders according to my scenes.  
&nbsp;&nbsp;For example, I have three scenes in my application which are named as MenuScene, ARScene, InformationScene  
&nbsp;&nbsp;thus I have ARSceneTextures, InformationSceneTextures, and MenuSceneTextures folders inside the Textures folder.  
  
&nbsp;&nbsp;A.2. General Structure of Scripts:  
&nbsp;&nbsp;I have ButtonStates folder which holds the information about the buttons on InformationScene,  
&nbsp;&nbsp;HandlingPlanetInformations folder which holds the content of the planets in InformationScene,   
&nbsp;&nbsp;ChangingButtonImageDynamically.cs file which changes the PlanetButton image in ARScene when the target image is found,   
&nbsp;&nbsp;HandlingButtonEvents.cs file which redirects application between scenes, PlanetRing.cs file which creates a ring for Saturn,   
&nbsp;&nbsp;Rotation.cs file which rotates planets around their center.  

B. Description of Application:  
&nbsp;&nbsp;First I created the MenuScene. MenuScene has Start and Exit buttons.   
&nbsp;&nbsp;When the start button is pressed, it goes to ARScene where image targets are recognized,  
&nbsp;&nbsp;and when the exit button is pressed, the application exits.   
  
&nbsp;&nbsp;Secondly, I created the ARScene. Since I use the Marker-Based Augmented Reality approach in my application,  
&nbsp;&nbsp;I have imported the Vuforia package into my application for the recognition of image targets.   
&nbsp;&nbsp;Then I used an AR Camera instead of the Main Camera. I put Image Targets in Vuforia's database   
&nbsp;&nbsp;and imported the database into my application. Then I used these image targets in my application.   
&nbsp;&nbsp;I placed planets on these image targets. I created three buttons on the left side of the screen in ARScene.   
&nbsp;&nbsp;When the home page button is pressed, the application is directed to the MenuScene, which is opened at first.   
&nbsp;&nbsp;When the Exit button is pressed, the application is terminated. When the Planet button is pressed,   
&nbsp;&nbsp;the planet information is transferred to the InformationScene according to the image target   
&nbsp;&nbsp;and the application is directed to the InformationScene, which contains the information of the planets.   
&nbsp;&nbsp;At the same time, the background image of the Planet button changes dynamically according to the planet recognized by the camera.   

&nbsp;&nbsp;Finally, I created the InformationScene. General information about the planets is shown here.   
&nbsp;&nbsp;There are five buttons in the InformationScene. When the Back button is pressed, the application is directed to ARScene.   
&nbsp;&nbsp;When the location information button is pressed, the planet's distance from the sun is displayed on the screen.     
&nbsp;&nbsp;When the Other informations button is pressed, detailed information about the planet is displayed on the screen.     
&nbsp;&nbsp;When the Left button is pressed, it switches between the other information pages to the left.        
&nbsp;&nbsp;When the Right button is pressed, it switches between the other information pages to the right.   
  
C. WARNING!!!    
&nbsp;&nbsp;After I finished my Unity application, I built this Unity project for the application to work on Android devices.   
&nbsp;&nbsp;In order for the mobile application to work on the Android platform, the Android version must be at least Android 6.0 (Marshmallow). 

D. Some Images From App:  

D.1. MenuScene  
![1](https://user-images.githubusercontent.com/76014928/146654323-27a71ca0-9436-438e-8a0f-2fc729ab48ef.png)

D.2. ARScene    
![2](https://user-images.githubusercontent.com/76014928/146654360-f24941fd-de3c-4124-9d19-7f232291b07d.png)
![3](https://user-images.githubusercontent.com/76014928/146654362-c386e2a3-6d5c-4177-b676-8dc6d43daefc.png)

D.3. InformationScene  
![4](https://user-images.githubusercontent.com/76014928/146654377-4ed4bc37-8088-4b0d-8e89-cbf845e34772.png)
![5](https://user-images.githubusercontent.com/76014928/146654380-23893e61-c2f7-4452-8cd6-ea89003110ad.png)
![6i](https://user-images.githubusercontent.com/76014928/146654381-1f0fb739-ac56-4824-a259-377755f1eb84.png)
![7](https://user-images.githubusercontent.com/76014928/146654387-1572a999-005e-4d87-80ec-8f0918ce5244.png)

