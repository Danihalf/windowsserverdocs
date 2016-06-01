---
title: Bitsadmin getowner
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 5203f84c-a879-4f31-ae3e-7ea74bd63ca5
---
# Bitsadmin getowner
Retrieves the owner of the specified job.

## Syntax

```
bitsadmin /GetOwner <Job>
```

## Parameters

|Parameter|Description|
|-------------|---------------|
|Job|The job's display name or GUID|

## <a name="BKMK_examples"></a>Examples
The following example displays the owner for the job named *myDownloadJob*.

```
C:\>bitsadmin /GetOwner myDownloadJob
```

## Additional references
[Command-Line Syntax Key](Command-Line-Syntax-Key.md)

