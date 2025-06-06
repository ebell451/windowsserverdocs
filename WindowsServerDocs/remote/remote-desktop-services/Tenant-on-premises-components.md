---
title: Tenant on-premises components
description: Describes the on-premises components in your RDS deployment.
ms.author: daknappe
ms.date: 7/3/2024
ms.topic: article
ms.assetid: b3eebb38-a835-4fa6-9e41-1966014bf2cb
author: robinharwood
manager: dongill
---
# Tenant on-premises components

The following information describes the on-premises components that make up the desktop hosting deployment.

## Clients

To access the hosted desktops and applications, the users must use Remote Desktop clients that support Remote Desktop Protocol (RDP) 7.1 or higher. In particular, the client must support Remote Desktop Gateway and Remote Desktop Connection Broker. To deliver applications to the local desktop, the client must also support the RemoteApp feature. To achieve highest gateway scale, the client must support the pure HTTP transport connections to RD Gateway.

Additional information:

- [Microsoft Remote Desktop Clients](./clients/remote-desktop-clients.md)
- [Remote Desktop app for Windows in Microsoft Store](https://apps.microsoft.com/windows/app/remote-desktop/051f560e-5e9b-4dad-8b2e-fa5e0b05a480)
- [Microsoft Remote Desktop - Android Apps on Google Play](https://play.google.com/store/apps/details?id=com.microsoft.rdc.android)
- [Mac App Store - Microsoft Remote Desktop](https://apps.apple.com/us/app/microsoft-remote-desktop/id1295203466?mt=12)
- [Microsoft Remote Desktop in the App Store](https://itunes.apple.com/app/microsoft-remote-desktop/id714464092?mt=8)

## Active Directory Domain Services

Some larger and more sophisticated tenants may choose to host an Active Directory Domain Services (AD DS) server on their premises. In this case, the AD DS server in the tenant's environment will typically be a replica of AD DS server that is on the tenant's premises. This is supported by creating a virtual network in the tenant's environment and using the Azure VPN to create a site-to-site connection from the tenant's on-premises network to the tenant's virtual network in the Azure data center.

Additional information:

- [Microsoft Azure Virtual Network Overview](/azure/virtual-network/virtual-networks-overview)
- [Create a resource manager VNet with a Site-to-Site VPN connection using the Azure portal](/azure/vpn-gateway/vpn-gateway-howto-site-to-site-resource-manager-portal)
