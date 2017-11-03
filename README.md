# SLA Manager

## Installation Guide

### Dependencies 

Install the dependencies 
- OS:
	- Windows 7 and newer
	- Windows Server 2008 R2 and newer
- [DotNetCore 1.1.4 Windows Hosting](http://download.microsoft.com/download/6/F/B/6FB4F9D2-699B-4A40-A674-B7FF41E0E4D2/DotNetCore.1.0.7_1.1.4-WindowsHosting.exe)
- [Internet Information Services Manager](https://docs.microsoft.com/en-us/aspnet/core/publishing/iis?tabs=aspnetcore1x)

To check that all the depencies have been set up, execute
```
  $ dotnet --version
  -> Microsoft .NET Core Shared Framework Host

		Version  : 1.1.0
		Build    : 928f77c4bc3f49d892459992fb6e1d5542cb5e86
```

### SLA Manager local set-up

To set the service, execute the following commands
``` 
  $ git clone https://github.com/sunfish-prj/SLA-Manager.git
  $ cd SLA-Manager
  $ dotnet Sunfish.SLAMService.dll
```
The server is now running and listening on the port chosen in the *hosting.json*. file (e.g. 80).  

The SLA Manager is expected to interact with the:
- [Registry Interface](https://github.com/sunfish-prj/Registry-Interface.git).

The *urls* and *ports* for the above application may be altered in the *appsettings.production.json* config file.
