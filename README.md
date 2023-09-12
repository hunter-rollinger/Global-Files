# Global-Files
The "Zenon" folder contains files used across all Zenon projects.  </br>

The "Fonts" folder contains all the required fonts for Zenon.  </br>

Both the "Add-ins" and "Tools" folders are copied from the vault.  </br>

CO_Example & GP_Example are both pulled from the CLi-100 Show Machine.  </br></br>


# Create From Template
1. Open the Git-Template repository on the GitHub web interface.  </br>

2. **Creating A New Repository**  </br>
   Click the green "Use this template" button and "Create a new repository".   </br>
   **DO NOT** check the "Include all branches" box. We'll add the experimental branch later.  </br>
   Name the repository as you see fit. Usually the name of the machine the project is based on.  </br>
   Make sure to the repository is private. We can add people to it later.  </br>
   
3. **Uploading Files**  </br>
   Now that you have a repository created we can upload files to it.  </br>
   The GitHub Desktop app is recommended for this as you can see the changes in real-time when you place files into the local cache.  </br>
   See [this](https://github.com/hunter-rollinger/Global-Files/tree/main#github-desktop-application) section for information on the desktop app.  </br>
   If you run into large file size issues see the [this](https://github.com/hunter-rollinger/Global-Files/tree/main#large-files) section for assistance.  </br>
   
4. **Creating The Experimental Branch**  </br>
   This will be used to push all future updates to so that there's always a stable version saved on production.  </br>
   Underneath your repository name at the top of the screen click where it says "1 branch".  </br>
   Click "New branch" at the top right of the screen, name it "experimental", and leave the source as "production".  </br>
   If using the GitHub Desktop app make sure to switch your current branch from production to experimental before pushing.  </br>

5. **Configure General Settings**   </br>
   Check the box next to "Discussions" under features.  </br>
   Un-Check the box next to "Projects".  </br>
   Scroll to the Archives section near the bottom.  </br>
   Check the "Include Git LFS objects in archives" box.  </br>

7. **Adding Collaborators**
   Click on the "Settings" tab in your GitHub repository.  </br>
   Click on "Collaborators" from the menu on the left side.  </br>
   Click the green "Add people" button.  </br>
   If the user has a GitHub account, type their username.  </br>
   Otherwise type in the email of the person you wish to add.  </br></br>

8. **Disable Actions**
   Click on the "Actions" dropdown on the leftside then "General".
   Click "Disable actions" under "Actions permissions".

10. **Discussions Setup**
   Under the "Discussions" tab click the pencil icon next to the "Categories" on the left side.
   Delete "Polls", "Q&A", and "Show and tell".
   On the main discussions page, click the "Label" button and "Edit labels".
   Delete "good first issue".
   Create "known issue" with description "The issue has been brought up or is known about" and color #71805B.


# Large Files
If the desktop app or web interface gives an error about large file sizes then the solution is to install Git LFS using GitHub CLI.  </br>

1. Download GitHub CLI
2. Open Git Bash in the directory where the desired GitHub repository is located.
3. Run the command "git lfs track {relative path/filename.extension}".
   - Example: git lfs track Add-Ins/WPF_Slider_App.zip  </br>
   
This command will create the necessary files for Git LFS to work with the repository.  </br>

Note: The only file that can be seen in the web interface is the ".gitattributes" file.  </br></br>


# GitHub Desktop Application
The GitHub Desktop Application is recommended for uploading files for initial machine uploads.  </br>

If the machine is currently being modified or a zenon program is being created for it then it is recommended for major revisions.  </br>

For small modifications the desktop application is not necessary as files can just be uploaded to the experimental branch.  </br>

GitHub CLI (Command Line Interface) is an alternative option for those interested.
