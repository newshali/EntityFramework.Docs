---
title: Design-time services - EF Core
description: Information on Entity Framework Core design-time services
author: bricelam
ms.date: 10/26/2017
uid: core/miscellaneous/cli/services
---
# Design-time services

Some services used by the tools are only used at design time. These services are managed separately from EF Core's runtime services to prevent them from being deployed with your app. To override one of these services (for example the service to generate migration files), add an implementation of `IDesignTimeServices` to your startup project.

[!code-csharp[Main](../../../../samples/core/Miscellaneous/CommandLine/DesignTimeServices.cs)]
