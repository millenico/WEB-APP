# escape=`

FROM mcr.microsoft.com/windows/servercore/iis

## Enable IIS Remote Management
#RUN powershell Install-WindowsFeature -Name Web-Mgmt-Service
#RUN powershell New-ItemProperty -Path HKLM:\SOFTWARE\Microsoft\WebManagement\Server -Name EnableRemoteManagement -Value 1 -Force


#RUN powershell -NoProfile -Command Remove-Item -Recurse C:\inetpub\wwwroot\*
 
## location of the source directory
WORKDIR /inetpub/wwwroot

COPY IIS-content/ .

## Give Full Access To Folder
# RUN icacls 'c:/inetpub/wwwroot' /grant 'Everyone:(OI)(CI)F'

## Check that the files have been successfully copied
RUN dir /a