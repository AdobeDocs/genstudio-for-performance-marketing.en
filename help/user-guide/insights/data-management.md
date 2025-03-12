---
title: Data management
description: Learn about data ingestion and storage for [!DNL Insights] in GenStudio for Performance Marketing.
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
---
# Data management

GenStudio for Performance Marketing uses Adobe Experience Platform (AEP) for data ingestion and storage of the metrics and metadata that power [!DNL Insights]. AEP uses _schemas_ to define the data structures and _datasets_ for storing and managing data collections.

## Data connections

GenStudio for Performance Marketing uses Customer Journey Analytics (CJA) to aggregate multiple data sources by creating a connection to one or more AEP datasets. CJA uses these data connections to create data views for analyzing metrics with [!DNL Insights].

>[!BEGINSHADEBOX]

**Important information about data connections**

If you are an [Adobe system administrator](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager), you may have entitlements that allow access to AEP sandbox management and data lake components that support GenStudio for Performance Marketing.

>[!WARNING]
>
>Resetting the production sandbox in AEP deletes all data connections and causes [!DNL Insights] to stop working.

Use caution and do not delete the following data connections required for GenStudio for Performance Marketing to operate reliably:

- AEP Datasets prefixed with `GS Insights`
- AEP Schemas, classes, and field groups prefixed with `GS Insights`
- Custom field group `timestamp for metadata`
- AEP Connections: data flows prefixed with `GS Insights`
- AEP Connections: GS Insights account

See [Delete implications](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) in the _Customer Journey Analytics_ guide before you delete any data components in AEP.

>[!ENDSHADEBOX]

## Data retention policy

GenStudio for Performance Marketing retains channel data for 13 months. This retention policy includes the 6 months of data ingested during the initial connection, ensuring comprehensive historical data analysis and reporting.

See [Connect channel ad account](/help/user-guide/insights/connect-channel.md).
