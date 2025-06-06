---
title: Sync your file server with the cloud by using Azure File Sync
description: Use Azure File Sync to centralize your organization's file shares in Azure, while keeping the flexibility, performance, and compatibility of an on-premises file server. Azure File Sync transforms Windows Server into a quick cache of your Azure file share with the optional cloud tiering feature.
ms.topic: article
author: davannaw-msft
ms.author: jgerend
ms.date: 04/12/2019
---
# Sync your file server with the cloud by using Azure File Sync

Use Azure File Sync to centralize your organization's file shares in Azure, while keeping the flexibility, performance, and compatibility of an on-premises file server. Azure File Sync transforms Windows Server into a quick cache of your Azure file share with the optional cloud tiering feature. You can use any protocol that's available on Windows Server to access your data locally, including SMB, NFS, and FTPS.

Once your files have synced to the cloud, you can connect multiple servers to the same Azure file share to sync and cache the content locally—permissions (ACLs) are always transported as well. Azure Files offers a snapshot capability that can generate differential snapshots of your Azure file share. These snapshots can even be mounted as read-only network drives via SMB for easy browsing and restore. Combined with cloud tiering, running an on-premises file server has never been easier.

Azure File Sync in Windows Admin Center is supported on Windows Server 2012 R2, Windows Server 2016, Windows Server 2019, Windows Server 2022, and Windows Server 2025.

For more info, see [Planning for an Azure File Sync deployment](/azure/storage/files/storage-sync-files-planning).
