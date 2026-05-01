---
title: Data Management
description: Learn about data ingestion and storage for [!DNL Insights] in GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
    internal-label: Integrations
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
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

See [Connect paid media account](/help/user-guide/connectors/connect-channel.md).
