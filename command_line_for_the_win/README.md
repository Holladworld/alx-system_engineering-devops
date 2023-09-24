# Command Line for the wing
CMD CHALLENGE is a pretty cool game challenging you on Bash skills. Everything is done via the command line and the questions are becoming increasingly complicated. It’s a good training to improve your command line skills!
- - - - - - - - - - - - -- - - - - - - - - - - - - - - - 

This project is NOT mandatory at all. It is 100% optional. Doing any part of this project will add a project grade of over 100% to your average. Your score won’t get hurt if you don’t do it, but if your current average is greater than your score on this project, your average might go down. Have fun!

## Table of Content
----------------------------------------
| Command line for the win		
| Table of content
| specific
| Refrences
| Challenge README.md file solution:   
| Steps I followed to complete the task|
-----------------------------------------

## Specific
In addition to completing the project tasks and submitting the required screenshots to GitHub, you are also required to demonstrate the use of the SFTP (Secure File Transfer Protocol) command-line tool to move your local screenshots to the sandbox environment.


## References :

SFTP Guide
SFTP File Transfer Tutorial
Here are the steps to follow:

Take the screenshots of the completed levels as mentioned in the general requirements.
Open a terminal or command prompt on your local machine.
Use the SFTP command-line tool to establish a connection to the sandbox environment. You will need the hostname, username, and password provided to you for the sandbox environment.
Once connected, navigate to the directory where you want to upload the screenshots.
Use the SFTP put command to upload the screenshots from your local machine to the sandbox environment.
Confirm that the screenshots have been successfully transferred by checking the sandbox directory.
Once the screenshots are transferred, you can proceed to push the screenshots to GitHub as mentioned in the initial requirements.
Make sure to include the steps you followed to use the SFTP command-line tool in your project’s README.md file. This will help the reviewers understand how you performed the file transfer using SFTP.
NOTE :
The screenshoots of completed level should be inside the dir /root/alx-system_engineering-devops/command_line_for_the_win/

# README File: steps I took to complete the task
 

- Take Screenshots:

Complete the levels as mentioned in the general requirements.
Take screenshots of the completed levels.
Prepare for SFTP:

Open a terminal or command prompt on local machine.
Establish SFTP Connection:

To use the SFTP command-line tool to establish a connection to the sandbox environment. You will need the following information:
Hostname: Provided to you for the sandbox environment.
Username: Your username.
Password: Your password.
Navigate to the Target Directory:

Once connected, navigate to the directory where you want to upload the screenshots within the sandbox environment.
Upload Screenshots:

Use the put command in SFTP to upload the screenshots from local machine to the sandbox environment. For example:
arduino
Copy code
put "C:/Users/hp/Desktop/ALX/1-next_9_tasks.png"
put "C:/Users/hp/Desktop/ALX/2-next_9_tasks.png"
Confirm Transfer:

NB: You may experience issue with the stroke /. windows uses backslash \ instead of forward slash. simply change it to forward slash. That is change this format ""C:\Users\hp\Desktop\ALX\2-next_9_tasks.png"" to this  "C:/Users/hp/Desktop/ALX/2-next_9_tasks.png". It will work


Confirm that the screenshots have been successfully transferred by checking the sandbox directory. You can do this by listing the files in the directory using ls or similar commands in SFTP.
Push to GitHub:

Once the screenshots are confirmed to be in the sandbox directory, you can proceed to push the screenshots to GitHub as mentioned in the initial requirements. This likely involves adding them to a Git repository, committing the changes, and pushing to the remote repository on GitHub.
Update README.md:


