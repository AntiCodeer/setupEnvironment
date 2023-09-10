# Step 1 : Download configuration
- [Choose your configuration.xml](https://config.office.com/deploymentsettings)
# Step 2 : Download Office Deployment tool
- [Download tool and extract the setup and configuration.xml in same diretory](https://www.microsoft.com/en-US/download/details.aspx?id=49117)
# Step 3 : Install the configuration with deployment tool
- Got to the direcrory with Admin CMD, type "setup /configure configuration.xml"
# Step 4 : Go to office installation directory
- Go the installation directory with "cd C:\Program Files\Microsoft Office\Office16"
# Step 5 : Perform the CMD commands
- Follow this commands

	- for /f %x in ('dir /b ..\root\Licenses16\ProPlus2021VL_KMS*.xrm-ms') do cscript ospp.vbs /inslic:"..\root\Licenses16\%x"


	- cscript ospp.vbs /setprt:1688
	- cscript ospp.vbs /unpkey:6F7TH >nul
	- cscript ospp.vbs /inpkey:FXYTK-NJJ8C-GB6DW-3DYQT-6F7TH
	- cscript ospp.vbs /sethst:e8.us.to
	- cscript ospp.vbs /act