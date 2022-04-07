
## VSTS

IIS Web Server


 
 
TFS AGENT-AWS
 
PAT

Prepare Target

Test-WSMan -ComputerName <<hostname>>

	•	Copy to target ConfigureWinRM.ps1	and  winrmconf.cmd
https://github.com/Microsoft/vsts-rm-documentation/tree/master/WinRM/WinRM-Http-Https-Without-Makecert

.\ConfigureWinRM.ps1 <<hostname>> http
.\ConfigureWinRM.ps1 <<hostname>> https
	•	Add Msdeploy location to PATH
	•	Create website entry on target IIS host manually=
	•	Enable Features:
https://stackoverflow.com/questions/20048486/http-error-500-19-and-error-code-0x80070021

	•	Change firewall settings of the host
https://forums.aws.amazon.com/thread.jspa?threadID=227958

Links
https://stackoverflow.com/questions/34055826/deploying-website-builds-to-azure-from-vsts-release-management


http://colinsalmcorner.com/post/end-to-end-walkthrough-deploying-web-applications-using-team-build-and-release-management


http://ec2-54-205-205-119.compute-1.amazonaws.com:8035/
