## Setting Up Git Aliases in PowerShell

# To configure custom Git aliases in PowerShell, follow these steps:

1. Open Your PowerShell Profile

To add custom aliases, you need to edit your PowerShell profile. Open it in a text editor by running:

```powershell
notepad $PROFILE


2. Add Custom Functions for Git Commands
In the profile file (Microsoft.PowerShell_profile.ps1), add the following functions to create Git command aliases:


function gst { git status }
function gpl { git pull }
function gps { git push }
function gd { git diff }
function gau { git add --update }
function gcm { git commit -v }
function gca { git commit -v -a }
function gb { git branch }
function gba { git branch -a }
function gco { git checkout }
function gcob { git checkout -b }
function gcot { git checkout -t }
function gcotb { git checkout --track -b }
function glog { git log }
function glogp { git log --pretty=format:"%h %s" --graph }

3. Save the Profile and Reload It
After adding the functions, save the profile file. To apply the changes in your current PowerShell session, run:

. $PROFILE

4. Verify the Aliases
You can now use the custom aliases in PowerShell. For example, you can use gst for git status, gpl for git pull, and gps for git push.
