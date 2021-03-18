# Git Kata: Configuring Git

This kata has no `setup.sh` script. Just read and follow along.

## Downloading and Installing Git on Windows

For North America resources:
* From the Stellantis VPN, download the Git install from the EUS site: http://eusportal/esd/Items/Details?PackageId=5233 
* Add the software to your cart, and checkout to order the install. It will take an hour or so for the install to complete.


For other regions:
* Download at https://git-scm.com/download/win (or use Chocolatey)
* Install using the pre-selected defaults (you may need administrative access for the install)


## Downloading and Installing Tortoise Git

TortoiseGit is a Windows Shell Interface to Git that makes Git usage easy for those who are comfortable with working in Windows. 

Install For North America resources:
* From the Stellantis VPN, download the Tortoise Git install from the EUS site: http://eusportal/esd/Items/Details?PackageId=5207
* Add the software to your cart, and checkout to order the install. It will take an hour or so for the install to complete.


Install for other regions:
* Download at https://tortoisegit.org/download/
* Install using the pre-selected defaults (you will need administrative access for the install)


### SSH authentication

SSH creates a secure connection from local computers to Github, making sure that only authorized persons can commit to your code repository. 

Follow the steps below ON THE STELLANTIS VPN to create your SSH key and configure Github using PuttyGen.

1. From Windows, run Start > Programs > TortoiseGit > Puttygen
2. In Puttygen, first click on the Generate button.
3. Move the mouse in the empty space to generate the Key.
4. Once the key is generated, copy the Public Key onto your clipboard. You'll use this later to authenticate. Leave the Key passphrase field blank. 
5. Next, click on the Save private key button. On the warning pop-up, click “Yes” and save your private key onto your system. Remember the name of this file.
6. Next, navigate to GitHub: https://github.intra.fcagroup.com/  and login using your LDAP credentials (TID).
7. In Github, in the top upper right hand corner click on your user account and choose settings.
8. Click on the SSH and GPG key menu on the left and click on New SSH key button.
9. Paste the Public Key copied from Step 4 into the Key section and give a title as shown below. (Title can be any name of your choice). Click on Add SSH Key to save your entry.
10. Open Windows explorer and create a new "git" folder under your C:\ drive. 
11. Right click on the folder and select Git Clone... from the context menu.
12. Enter the following in the URL: box: https://github.intra.fcagroup.com/FCA-PROPULSIONSYSTEMS/GIT_Training.git 
13. Select the Load Putty Key checkbox, and select the ppk file you saved in step 5.
14. Select OK and you should see the repo being cloned (downloaded) locally to your machine. It should show a success message once complete. Close the dialog box.

Git and Tortoise Git are now authenticated to Stellantis Enterprise Github.
 
