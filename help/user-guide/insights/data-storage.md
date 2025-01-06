---
title: Data storage
description: Learn about data storage for Insights in GenStudio for Performance Marketing.
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
---
# Data storage

GenStudio for Performance Marketing uses Adobe Experience Platform (AEP) to store data, such as the metrics and metadata that power Insights. If you are an [Adobe system administrator](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager), you may have entitlements that allow access to AEP data lake components that support your GenStudio for Performance Marketing application.

The following structures are required for GenStudio for Performance Marketing to operate reliably and should **NOT** be deleted:

- AEP Datasets prefixed with `GS Insights`
- AEP Schemas, classes, and field groups prefixed with `GS Insights`
- Custom field group `timestamp for metadata`
- AEP Connections: data flows prefixed with `GS Insights`
- AEP Connections: GS Insights account
