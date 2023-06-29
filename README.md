# Solar System AR
A. General Structure of Application:  
<br>
A.1. General Structure of Folders:  
I have grouped my application files structured inside the DataFiles folder.  
I have Animations, Audios, Fonts, Logo, Materials, Scenes, Scripts, and Textures folder in the DataFiles folder.  
I also structured each of these subfolders according to my scenes.  
For example, I have three scenes in my application which are named as MenuScene, ARScene, InformationScene  
Thus I have ARSceneTextures, InformationSceneTextures, and MenuSceneTextures folders inside the Textures folder.  
  
<br>
A.2. General Structure of Scripts:  
<br>
I have a ButtonStates folder which holds the information about the buttons on InformationScene,  
<br>
HandlingPlanetInformations folder which holds the content of the planets in InformationScene,   
<br>
ChangingButtonImageDynamically.cs file which changes the PlanetButton image in ARScene when the target image is found,   
<br>
HandlingButtonEvents.cs file which redirects applications between scenes, PlanetRing.cs file which creates a ring for Saturn,   
<br>
Rotation.cs file which rotates planets around their center.  

B. Description of Application:  
<br>
First I created the MenuScene. MenuScene has Start and Exit buttons.   
When the start button is pressed, it goes to ARScene where image targets are recognized,  
and when the exit button is pressed, the application exits.   
  
<br>
Secondly, I created the ARScene. Since I use the Marker-Based Augmented Reality approach in my application,  
<br>
I have imported the Vuforia package into my application for the recognition of image targets.   
<br>
Then I used an AR Camera instead of the Main Camera. I put Image Targets in Vuforia's database   
<br>
and imported the database into my application. Then I used these image targets in my application.   
<br>
I placed planets on these image targets. I created three buttons on the left side of the screen in ARScene.   
<br>
When the home page button is pressed, the application is directed to MenuScene, which is opened first.   
<br>
When the Exit button is pressed, the application is terminated. When the Planet button is pressed,   
<br>
the planet information is transferred to the InformationScene according to the image target   
<br>
and the application is directed to the InformationScene, which contains information about the planets.   
<br>
At the same time, the background image of the Planet button changes dynamically according to the planet recognized by the camera.   

<br>
Finally, I created the InformationScene. General information about the planets is shown here.   
<br>
There are five buttons in the InformationScene. When the Back button is pressed, the application is directed to ARScene.   
<br>
When the location information button is pressed, the planet's distance from the sun is displayed on the screen.     
<br>
When the Other information button is pressed, detailed information about the planet is displayed on the screen.     
<br>
When the Left button is pressed, it switches between the other information pages to the left.        
<br>
When the Right button is pressed, it switches between the other information pages to the right.   
<br><br>
C. WARNING!!!    
<br>After I finished my Unity application, I built this Unity project for the application to work on Android devices.   
<br>In order for the mobile application to work on the Android platform, the Android version must be at least Android 6.0 (Marshmallow). 

D. Some Images From the App:  

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
