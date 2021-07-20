# Project_Final_Year
Multiple Face recognition based Attendance System

# Author's Identity
## Team Members
	**Arpit Pathak (1701410034) arpitpathak114@gmail.com**
	**Pratishtha Agarwal (1701410078) pratishtha013@gmail.com**
	**Shivi Saxena (1701410096) Saxenashivi20@gmail.com**
## Supervisor's Name
	**Mr. Hiresh Kumar Gupta**
	**Assistant Professor (Department of Computer Science and Engineering)**
	**Shri Ram Murti Smarak College of Engineering and Technology, Bareilly.**



# Files in CD
	## Documentation
		**Project presentation: A presentation showing the details about the project with flowchart.**
		**README.md: File having Author's identity, System requirements and Steps to run the project**
	## Project_Deployment : Project Folder
		**app.py: Main file to run the web portal**
		**database_create.sql: sql file containing queries to create database**
		**dataset_prepare.py: (Not to be edited) module to prepare dataset from uploaded dataset of student**
		**modelTrain.py: (Not to be edited) module to train the model over the dataset**
		**recognition.py: (Not to be edited) module to recognize the faces from the video uploaded by faculty**
		### Templates: Folder containing UI templates for project**



# System Requirements
	## Hardware Requirements
		**Intel core i3**
		**4GB RAM**
		**50GB Hard Disk**
	## Software Requirements
		**Python 3.4+ Installed and added to path.** [Download Python](https://www.python.org/downloads/)
		**MySQL 8.0(GA) installed in system and setup on port number 3306.** [Download MySQL](https://www.mysql.com/downloads/)
		**MySQL Workbench should be ready to create database.**



# Steps to Setup the Project
1.	Copy the whole folder **Project_deployment** in your system as it is.
2.	Open command prompt, move to the path of your project folder and run command **pip install -r requirements.txt**.
3.	Open MySQL workbench and import database_create.sql file in the project folder. Run the file to create the database. You can change the admin login details in the last query.
4.	Now open **app.py** file in any IDE or editor (Notepad/Sublime/VS Code etc.). Change the **user** and **password** in line number 23 as you setup for your MySQL server.



# Steps to run the project
1.	You can run the project either on local server or on ngrok server.
	>	***To run on local server-*** **Double click app.py**. To disable debug mode, remove **debug=True** from last line on app.py and then run the file.
	>	Terminal will open showing the local ip address (ex. 127.0.0.1:5000).
	>	Open this ip address in your browser and interact with attendance portal.
	>	This link will work only on the device where the file is running i.e your local server.
	>	Note: This will only run the web app on your local server. 
	
	(Recommended to run the portal on ngrok so that it is accessible from any device)
	>	To run on ngrok server *uncomment the line __#run_with_ngrok(app)__ as __run_with_ngrok(app)__*.
	>	Remove **debug=True** from last line of app.py. Save it and double click the file. 
	>	Terminal will open showing the http and https links. Copy any of your link in browser to interact with the attendance portal.
	>	This link can be used from any device connected to internet.

2.	Once you are on the Login page, Login as Admin with the username and password as in the last line of database_create file.
	>	Go to Add record and add username(Name) and password (id) for student and faculty to enable login for them.
	>	Now give the website link to students and faculties to login with their username and password and register themselves on the portal.
	>	Faculties have to register by only mentioning their department.

3.	**Student Registration**: Students have to upload a zip file containing 25 of their front_facing photos. 
	***Make sure the photos have full face of student and background is clear***

4. After all students for a particular class have registered. Login as admin and train the model for that particular class from dashboard.

5. The faculty will upload a mp4 video of about 30 to 45 seconds of the class students on the portal along with date to mark their attendance.

6. Faculties can also edit the attendance in the Edit attendance tab.

7. Students can login and see their attendance on the dashboard a well as track their attendance datewise.
	

	
	
	
