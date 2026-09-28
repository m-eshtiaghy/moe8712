General-Purpose Tools

1. Using PSADT deployment toolkit Reference · [PSAppDeployToolkit](https://psappdeploytoolkit.com/docs/3.10.2/reference)  created a package

As for the tool, it is PSADT, and not the latest 4.x but the previous 3.1.x version. 
I used this tool for years, it is basically a powershell based wrapper, handles UAC elevation, has its own set of commands to simply make registry changes, exe/msi installations, and also open to use any powershell script inside the allowed parts (it has sections for Pre-Install - Install - Post Install (as well as uninstall and repair).
The nice thing with it is that it comes with a deploy-applicaiton.exe that the user can run himself and it will prompt for elevation and run the whole toolkit, with nice window prompts and progress. Also logging is built in, to a chosen folder (I usually do c:\programdata\[company] ). 
Note: it is a wrapper, not a repackager, so it does not need to be 'compiled'. It has folders for installer files and the toolkit's files, all of it has to be shared and the user can run the deploy-application. In Intune, it works the same way but with a silent install/uninstall switch and it goes silent, but logs the same way on the client.




