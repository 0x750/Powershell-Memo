# Introduction

From the Microsoft [What is PowerShell ?](https://docs.microsoft.com/en-us/powershell/scripting/) introduction :

> PowerShell is a cross-platform task automation and configuration management framework, consisting of a command-line shell and scripting language. Unlike most shells, which accept and return text, PowerShell is built on top of the .NET Common Language Runtime (CLR), and accepts and returns .NET objects. This fundamental change brings entirely new tools and methods for automation.

## How to use PowerShell

### How to launch a PowerShell window

To launch PowerShell, you can search for "PowerShell" in the Windows Menu, or from the `Windows key` + `x` menu, and then hit the underlined key for PowerShell. From there you can start to enter commands or run scripts.

A blue window should appears with the following text and a cursor :

```powershell
Windows PowerShell
Copyright (C) Microsoft Corporation. All Rights reseved.

PS C:\Users\yourUsername>
```

### Basic commands

Every cmdlet or function in PowerShell is named as follow : `Verb-Noun`.

To get the list of avaible commands :

```powershell
Get-Command
```

> Depending on your PowerShell modules, this command can output a massive list of commands, we will see later how to search efficiently and filter the output.

To see the documentation of any command :

```powershell
Get-Help Any-Command
```

To get the full path of the current directory :

```powershell
Get-Location
```

To change the working directory :

```powershell
Set-Location .\Relative\Path\...
Set-Location ..\..\Relative\Path\...
Set-Location C:\Full\Path\...
```

To list the content of the current directory :

```powershell
Get-ChildItem
```

To get on item :

```powershell
Get-Item .\Path\To\Item
```

To set a variable and output the value of a variable to the console :

```powershell
$CurrentDir = Get-Location
$CurrentDir
```

This code will output the value returned by the `Get-Location` command.

