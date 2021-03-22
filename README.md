# Git and Git-hub set-up guide

## Setup
- Have Git installed on your computer
- Create a Github account
* Generate an SSH key to allow your local machine to push changes to your Github account by typing ```ssh-keygen -t ed25519 -C "your_email@example.com"```, making sure that the email you enter is the same as the one in your Github account
 * enter ```cd ~/.ssh ```
 * ```ls```
 * a file named ```id_rsa.pub``` should be present, open it via text editor (like by entering ```cat id_rsa.pub```) and copy its contents
 * go to your user profile on Github, enter the settings, go to the "SSH and GPG keys", and add the SSH key you just copied in the appropriate input field

## Steps
- the first thing you need to do is create a folder for your project on your machine
- make sure that the name of the folder (and the repository in general) is appropriately formatted following conventions, like using underscore instead of whitespaces
- Open the command prompt (on Windows) or the Terminal (on Linux and Mac), and type ```cd <path to my_repository folder>```
- Initialise the repository with ```git init```
- In this folder, create a file called README.md via the command ```touch README.md```
- Edit the contents of the file with the text editor of your choice
- You can create any other file the same way, a very important file is ```.gitignore```, that allows git to ignore certain files during update
- add the files you created to the temporary repository by using ```git add <name of the file>```, you can check the status of your repository by typing ```git status```
- write a description of the commit you're submitting with ```git commit -m "description of the commit"```
- type ```git config --global user.email "<your_email@example.com>"```
- finally ```git push -u origin main```
- Done!
