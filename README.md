# Voice_Recognition_And_Face_Recognition_System
Implement voice biometric and face recognition system for authentication for security.<br><br> 
Consider there is a door with access control which can be unlocked with your voice and face. Prepare database/model with your face and voice data. When you reach at access control system, you have to speak your name which activates the voice biometric authentication, identifies that it is your voice then captures your photo. Photo is again compared with existing database/model for verification. If any of the 2 authentication fails, door is not unlocked. Both methods need to be successful in order to unlock the door.<br> 

Steps for running application on Windows Platform
===================================================
Note: Please skip skip these steps which already you have. 
      A general guide for installation & running application. 

1) Install Anaconda on Windows Platform.<br>
   Help link: https://medium.com/@neuralnets/beginners-quick-guide-for-handling-issues-launching-jupyter-notebook-for-python-using-anaconda-8be3d57a209b
 
2) Open Jupyter Notebook from Anaconda Navigator or Terminal. (Two ways to open Jupyter Notebook) <br>
   Help link: https://medium.com/@neuralnets/beginners-quick-guide-for-handling-issues-launching-jupyter-notebook-for-python-using-anaconda-8be3d57a209b

3) Install Required Python Packages on Windows Platform.

   Package Name: mysql-connector<br>
   Just type the command into your terminal: pip install mysql-connector

   Package Name: SpeechRecognition<br> 
   Type Command into Terminal: pip install SpeechRecognition

   Package Name: PyAudio<br>
   Type Command into Terminal: pip install pyaudio   
 
   Package Name: DLib<br>
   Type Command into Terminal: pip install dlib

   Package Name: Pillow<br>	
   Type Command into Terminal: pip install pillow
   
   Face Recognition<br>
   pip3 install face_recognition

4) Install XAMPP on Windows Platform.<br>
   Help Link: https://www.wikihow.com/Install-XAMPP-for-Windows

5) Import "ai-demo" database into XAMPP/WAMP/LAMP.<br>
   Help Link: https://www.youtube.com/watch?v=7WUw9J3Xs8Q
 
6) In Jupyter Notebook Select File Menu.<br>
   Help link: https://medium.com/@neuralnets/beginners-quick-guide-for-handling-issues-launching-jupyter-notebook-for-python-using-anaconda-8be3d57a209b 

7) Find file call "VR_And_FR_System.ipynb" into Jupyter Notebook. Just Click on that File. It will opens into Jupyter Notebook.

8) Specify the image path according to your system. (In my system I have stored all the images: "C:/Users/Pritul/Pictures/Camera Roll/")

9) Specify mysql username and password according to your system. (In my system: msqlconn.connect(host="localhost",user="*****",passwd="*****",database="ai_demo"))

9) Plug the Microphone into your computer.

10) Choose Kernal from the Menu option in Jupyter Notebook > Select Restart & RunAll option.



Tested cases & result screen shot
===================================
case 1 : When we have not pluged microphone then what will happen ?

case 2: When we have plugged the microphone, I am not speaking then what will happen?

case 3: When Apache & Mysql is not running then what will happen?

case 4: When we have plugged the microphone, I am speaking full name which does not exist into our database then what will happen?

case 5: When we have plugged the microphone, I am speaking more than 2 names then what will happen?

case 6: When we have plugged the microphone,   I am speaking name only which is not exists in our database then what will happen?

case 7: When we have plugged the microphone,   I am speaking name only database name and speaking name is in the different case then what will happen?

case 8: When we have plugged the microphone,  I am speaking name only and around me so much noise like(playing a song, any loud sound) then what will happen?

case 9: when we have plugged the microphone,  I am speaking name as "Maulik" but I am matching "Praful" face then what will happen?

case 10: When we have plugged the microphone,   I am speaking name as "Obama" but I am matching "Obama" face via Mobile phone then what will happen?
