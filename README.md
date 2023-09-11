# Global-Files
The "Zenon" folder contains files used across all Zenon projects.  </br>

The "Fonts" folder contains all the required fonts for Zenon.  </br>

Both the "Add-ins" and "Tools" folders are copied from the vault.  </br>

CO_Example & GP_Example are both pulled from the CLi-100 Show Machine.  </br></br>

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
