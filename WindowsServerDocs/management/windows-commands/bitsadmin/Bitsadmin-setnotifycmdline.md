---
title: Bitsadmin setnotifycmdline
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 415ae6ef-8549-48b2-9693-2368a6e24075
---
# Bitsadmin setnotifycmdline
Sets the command\-line command that will run when the job finishes transferring data or when a job enters a state..

## Syntax

```
bitsadmin /SetNotifyCmdLine <Job> <ProgramName> [ProgramParameters]
```

## Parameters

|Parameter|Description|
|-------------|---------------|
|Job|The job's display name or GUID|
|ProgramName|Name of the command to run when the job completes.|
|ProgramParameters|Parameters that you want to pass to *ProgramName*.|

## Remarks
You can specify NULL for *ProgramName* and *ProgramParameters*. If *ProgramName* is NULL, *ProgramParameters* must be NULL.

> [!IMPORTANT]
> If *ProgramParameters* is not NULL, then the first parameter in *ProgramParameters* must match *ProgramName*.

## <a name="BKMK_examples"></a>Examples
The following example sets the command\-line command used by the service to run notepad when the job named *myDownloadJob* completes.

```
C:\>bitsadmin /SetNotifyCmdLine myDownloadJob c:\winnt\system32\notepad.exe NULL
```

```
C:\>bitsadmin /SetNotifyCmdLine myDownloadJob c:\winnt\system32\notepad.exe "notepad c:\eula.txt"
```

## Additional references
[Command-Line Syntax Key](Command-Line-Syntax-Key.md)

