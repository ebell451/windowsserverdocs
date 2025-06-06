---
title: bitsadmin sethelpertokenflags
description: Reference article for the bitsadmin sethelpertokenflags command, which sets the usage flags for a helper token that is associated with a BITS transfer job.
ms.topic: reference
ms.author: mosagie
author: robinharwood
manager: mtillman
ms.date: 03/01/2019
---

# bitsadmin sethelpertokenflags

Sets the usage flags for a [helper token](/windows/win32/bits/helper-tokens-for-bits-transfer-jobs) that is associated with a BITS transfer job.

> [!NOTE]
> This command isn't supported by BITS 3.0 and earlier.

## Syntax

```
bitsadmin /sethelpertokenflags <job> <flags>
```

### Parameters

| Parameter | Description |
| --------- | ----------- |
| job | The job's display name or GUID. |
| flags | Possible helper token values, including:<ul><li>**0x0001.** Used to open the local file of an upload job, to create or rename the temporary file of a download job, or to create or rename the reply file of an upload-reply job.</li><li>**0x0002.** Used to open the remote file of a Server Message Block (SMB) upload or download job, or in response to an HTTP server or proxy challenge for implicit NTLM or Kerberos credentials.</li></ul>You must call `/setcredentialsjob targetscheme null null` to send the credentials over HTTP. |

## Related links

- [Command-Line Syntax Key](command-line-syntax-key.md)

- [bitsadmin command](bitsadmin.md)
