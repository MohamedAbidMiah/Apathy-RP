# Apathy SMP Mircs
This is used to help manage the Apathy smp for mircs. It uses docker to run a multi network server and then deploys it to an oracle server with GitHub actions. 

# For developers 
Make all changes for config in /config. Make and commit files and folders if necessary. 

When testing locally and making changes to /config, make sure to ran a bash or bat file to sync changes to source code.

## Example
```
@echo off
echo Copying local configs to data folder...
xcopy /s /y /i "configs\survival" "data\survival\plugins"
xcopy /s /y /i "configs\survival" "data\survival-2\plugins"
xcopy /s /y /i "configs\proxy" "data\proxy\plugins"

echo Done! Server is updating/starting.
pause
```
# Branching
All new features or issues should have a separate branch.

https://medium.com/@abhay.pixolo/naming-conventions-for-git-branches-a-cheatsheet-8549feca2534

# Committing 
Make sure the commit message explain what the code does and what you are trying to achieve. 

https://www.conventionalcommits.org/en/v1.0.0/

# Warning
All commits should follow this guide or it will automatically get rejected. 
