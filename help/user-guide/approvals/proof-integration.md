---
title: Workfront Proof integration with review and approvals
description: Workfront Proof integration with Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
---
# Workfront Proof integration with GenStudio for Performance Marketing

Integration with Workfront Proof enhances the GenStudio for Performance Marketing review-and-approval lifecycle with advanced features, including approval templates, multi-stage workflows, and the ability to [compare proof versions](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs). This structured versioning ensures transparency, accountability, and streamlined collaboration throughout the content review lifecycle.

>[!BEGINSHADEBOX]

**Prerequisites**:

Install the [Adobe Workfront Web Viewer extension](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

Workfront Proof's [!DNL Proofing Viewer] is a rich workspace for viewing, commenting on, and comparing proofs. From [!DNL Proofing Viewer], you can 

* Compare different versions of the content
* Add comments and drawing markups to a proof
* Approve the proof

[!DNL Proofing Viewer] loads when you click on the proof URL in your approval request email or in-product notification. The [!DNL Proofing Viewer] _My new approval_ view opens. From this view, you can review content and provide comments using the core [!DNL Proofing Viewer] annotation tools. 

To exit [!DNL Proofing Viewer], click **[!UICONTROL Return to GenStudio]**.

## Genstudio for Performance Marketing and Workfront Proof: feature comparison

The table below compares the standard GenStudio for Performance Marketing review-and-approval features to the more advanced capabilities available through the Workfront Proof integration.

| Feature        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Draft/proof lifecycle**        | Draft content expires upon publication. | Multi-stage, role-based approval chains with timestamped, persistent logs.<br> All versions are retained indefinitely.|
| **Comments**                | Comments are tied to draft ID and discarded after publication.                                           | Persistent comments and annotations are retained for audit and compliance.     |
| **Versions**           | Drafts are treated as unique instances.<br>No side-by-side comparison.                                      | Full version control with side-by-side and overlay comparison tools.        |
| **Project management**    | Basic campaign management.  | Full campaign lifecycle management, including customization, templates, reporting, and detailed audits. |

### Licenses and user roles

Licenses identify the set of user entitlements within a product. Workfront Proof provides more license types or user roles than GenStudio for Performance Marketing. [Proof roles overview](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) introduces user roles associated with the Workfront Proof review-and-approval workflow.

| GenStudio for Performance Marketing license       | Workfront license                 | Description                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Workfront Administrator/Power User | Full access to GenStudio Performance Marketing features such as brand, persona, and product management. Manages workflows and settings. Creates approval templates. |
| Content creator and editor (Power user license)   | Proof Creator (Standard license)  | Generates and submits content drafts. In Proofing Viewer, uploads assets and initiates proofs. Requires a Workfront Proof license.                              |
| Reviewer / Approver (Collaborator license)        | Reviewer/Approver                 | Participates in multi-stage reviews, adds comments, and approves or rejects content.                                                                             |

Adobe system administrators manage user provisioning and entitlements for both products in the Adobe Admin Console.

>[!NOTE]
>
> Workfront Proof provides [additional user roles](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles). Not all roles are visible inside of Performance Marketing. However, the system honors any role set inside a Workfront Proof template.

### Drafts and proofs

Workfront [!DNL Proofing Viewer] extends GenStudio for Performance Marketing's basic review-and-approval process with more structured review-and-approval features. Proofs reviewed in this integration are limited to the formats supported by GenStudio for Performance Marketing.

### Version control

GenStudio for Performance Marketing does not support approval templates, but WorkFront Proof does. Proof's versioning capabilities significantly enhance GenStudio's content review-and-approval process. Each submission in the Proof workflow is treated as a distinct version of the content draft or _proof_. Proofs are automatically saved and can be compared side-by-side with previous iterations. Stakeholders can track changes, provide precise feedback, and maintain alignment throughout the review cycle. Proof preserves a complete history of all comments, decisions, and versions, supporting audit readiness and compliance requirements. Each version also supports multi-stage, role-based approval workflows, with every action—approval, rejection, or comment—clearly logged and timestamped.

### Approval templates

Workfront Proof approval templates provide preformatted steps that can streamline the proof approval workflow. These templates include selected reviewers and approvers, proof roles, and deadlines, ensuring consistency and efficiency. Content creators launching a review can select from a set of predefined templates for both single-phase and multi-phase approval workflows. 

Each stage of the workflow template identifies assigned reviewers. All status updates and comments from the Workfront Proof workflow are visible within the Proofing Viewer, enhancing transparency and collaboration.

Approval templates support multi-stage approvals, which support the coordination of reviews from different groups of stakeholders.

### Comments

Reviewers can click directly on specific areas of the proof to leave precise, contextual comments. All comments are timestamped and saved as part of the proof's version history. Comment history is not available in GenStudio for Performance Marketing.

You can [compare two versions of a proof](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) to evaluate review comments and content.

## Notifications and reminders

Reviewers and approvers receive email notifications when a new proof is available for review or when an ongoing review has changed status. 
[Proof notifications and reminders](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders) include a personalized link to the proof, details about the proof and its progress through the approval process, and versioning information.
