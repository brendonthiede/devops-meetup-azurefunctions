# Azure Functions: Serverless Development Concepts

This is for the June 5, 2018 Lansing DevOps Meetup

## Summary

VMs allowed organizations to split up their infrastructure into easier to manage, more flexible pieces.
Docker and other containerization technologies allowed us to have even lighter weight deployment units while keeping isolation between processes.
"Function as a Service" technologies like AWS Lambda, Azure Functions, and Open Whisk allow for even more fine grained deployment unit.
Smaller units of deployment can give cloud providers better hardware utilization, which can result in huge savings for customers.

But with each new model of deploying apps comes a new way of developing and managing apps.
Microsoft's Azure Functions was later to the game than AWS Lambda, but they have tried to focus on creating a better developer experience.

## Prerequisites for running Azure Functions locally

### .NET Core

Install .NET Core 2.0 or later: https://www.microsoft.com/net/download/windows

### Azure Functions CLI

Requires Node 6.0 or later

```powershell
npm install -g azure-functions-core-tools@core
```

### Azure Storage Emulator

The Azure Storage Emulator can be downloaded as a standalone (as of 5/25/2018: https://go.microsoft.com/fwlink/?linkid=717179&clcid=0x409), or as part of the Microsoft Azure SDK.  Azure Storage Emulator uses LocalDB behind the scenes, so you may also need to install the latest SQL Server Express with LocalDB features enabled.  One installed, be sure to initialize storage.  Instructions are here: https://docs.microsoft.com/en-us/azure/storage/common/storage-use-emulator

You will benefit from also installing the Microsoft Azure Storage Explorer: https://azure.microsoft.com/en-us/features/storage-explorer/
