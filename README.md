# sidewalk-starter-site
Sidewalk Web Dev – Starter Website Template

This repository is the base starter template used by Sidewalk Web Dev to build fast, clean, and responsive websites for clients.

The goal of this template is to provide a consistent structure that can be easily customized for each client while keeping development and updates simple.

WHAT THIS TEMPLATE IS FOR

• Static websites for local businesses
• Fast setup for new client projects
• Easy collaboration using GitHub
• Simple deployment with Netlify

Clone this template for each new client project and customize it with each client's branding, content, and images.

HOW TO CLONE THIS TEMPLATE

Clone the repository from the Sidewalk Web Dev GitHub organization.

Rename the project folder to match the client’s name.

Open the project in VS Code.

Create a new GitHub repository for the client under the Sidewalk Web Dev organization and push this project to that repository.

DEVELOPMENT NOTES

• Use Live Server in VS Code to preview changes locally
• Keep styles clean, readable, and organized
• Commit changes frequently with clear commit messages
• Use feature branches when collaborating

FULL CLONING TUTORIAL:

CREATING THE TEMPLATE FOLDER:

on your latop create a folder and name it "sidewalk-web-dev-projects"

open your terminal and enter in the command "cd desktop"

following this, enter the command "cd sidewalk-web-dev-projects"

now that you're in the folder, clone the repository by entering the command
git clone (repository link)
example:  git clone https://github.com/sidewalk-web/sidewalk-starter-site.git

DUPLICATING THE TEMPLATE FOLDER:

now you can simply go into the folder on your desktop, copy and paste the 
"sidewalk-web-dev-projects" folder, and rename it to the new client

this folder is still linked to the starter template repository, so now we
will disconnect it

DISCONNECTING THE NEW FOLDER:

at this point in the terminal you should be in the sidewalk-web-dev-projects folder,
it should appear as: yourname@Mac sidewalk-web-dev-projects %
enter the commmand "cd (yourprojectname)"
example: cd la-prime-cafe-website
following this, enter the command: "git remote -v"
this will tell you if the proejct is linked to a repository, if it is it should say:
origin	https://github.com/sidewalkwebdev/sidewalk-starter-site.git (fetch)
origin	https://github.com/sidewalkwebdev/sidewalk-starter-site.git (push)

if it says this, enter the command "git remote remove origin"

now the folder is disconnected from the original repo it was copied from

MAKING IT ITS OWN REPO:

now go to the github organization and create a new repository, make sure it has the
same name as the folder you just made
do NOT add a README

now go back into the terminal and enter this command:
git remote add origin (repository link)
git branch -M main
git push -u origin main

you are now done and can open the new project folder in vscode
