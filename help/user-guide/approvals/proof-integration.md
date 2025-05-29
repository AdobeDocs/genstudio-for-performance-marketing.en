---
title: Workfront Proof integration with review and approvals
description: Workfront Proof integration with Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
---
# Workfront Proof integration with GenStudio for Performance Marketing

Integration with Workfront Proof enhances the GenStudio for Performance Marketing review and approval lifecycle with advanced features, including approval templates, multi-stage workflows, and the ability to compare draft (proof) versions.

>[!BEGINSHADEBOX]

**Prerequisites**:

Install the [Adobe Workfront Desktop Proofing Viewer extension](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension).

>[!ENDSHADEBOX]

## Get started

Proofing Viewer loads when you click on the proof URL in your approval request email or in-product notification. The Proofing Viewer _My new approval_ view opens. 

### Proofing Viewer

Proofing viewer is a rich workspace for viewing, commenting on, and comparing proofs. 

From Proofing Viewer, you can 

* Compare different versions of the content
* Add comments to a draft, or proof
* Approve the proof

Click **[!UICONTROL Return to GenStudio]** to return to exit Proofing Viewer and return to the GenStudio for Performance Marketing Canvas.

## Feature comparison overview

High-level comparison of GenStudio for Performance Marketing and Workfront Proofing Viewer features

| Feature        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Draft vs proof**            | Each asset or experience is a draft with a unique ID                                      | Each asset or experience is uploaded as a proof                                |
| **Draft/proof lifecycle**        | Only designated approvers can finalize a draft for publication<br>Draft ID and comments expire upon publication | Multi-stage, role-based approval chains with timestamped, persistent logs<br> All versions and comments are retained indefinitely                                              |
| **Comments**                | Comments are tied to draft ID and discarded after publishing                                           | Persistent comments and annotations are retained for audit and compliance           |
| **Versions**           | Drafts are treated as unique instances<br>No side-by-side comparison                                       | Full version control with side-by-side and overlay comparison tools             |

### Drafts and proofs

Workfront Proofing Viewer extends GenStudio for Performance Marketing's basic review-and-approval process with more structured review and approval features. Proofs reviewed in this integration are limited to the formats supported by GenStudio for Performance Marketing.

The following table summarizes the high level differences between GenStudio for Performance Marketing drafts and Workfront proofs. 


| Feature                   | GenStudio for Performance Marketing                                                                 | Workfront Proof                                               |
|---------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|
| **Versions**            | Tracks unique draft IDs with version history and status logs.<br>Draft IDs and URLs expire when the draft is published. | Robust version control with side-by-side comparisons           |
| **Comments**            | Threaded comments across teams (creative, legal, etc.).<br>Comments not saved after publication.     | Real-time, threaded comments with tagging and alerts           |
| **Markup tools**          | Limited markup                                                                                       | Rich markup tools (highlight, draw, pin, and strikeout)        |
| **Draft and proof lifespan** | Drafts expire post-approval                                                                      | Proofs are versioned with audit trails and history             |
| **Storage after approval**| Saved in Content. Review comments not retained                                                       | Saved in Workfront DAM or external repositories                |
| **Staged approvals**      | Only one approval stage                                                                              | Multiple approval stages                                       |


Proofing Viewer supports these additional tasks:

* [Compare two versions of a proof](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs#comparing-proof-versions)

* Access comments for published content

### User roles

Workfront Proof provides a more granular set of user roles than GenStudio for Performance Marketing. 

| GenStudio Role               | Workfront Proof Role     | Description                                                                 |
|-----------------------------|----------------------------------|-----------------------------------------------------------------------------|
| **GenStudio System Manager**   | Workfront Administrator/Power User | Full access to Genstudio Performance Marketing features such as brand, persona, and product management. Manages workflows and settings. Creates approval templates |
| **Content editor (Power user)**       | Proof Creator/Uploader       | Generates and submits content drafts. In Proofing Viewer, uploads assets and initiates proofs. |
| **Reviewer/Approver**        | Reviewer/Approver            | Participates in multi-stage reviews, adds comments, and approves or rejects content. |
| **Collaborator/Commenter**   | Commenter                      | Can view and comment on drafts or proofs, but cannot approve or reject.     |

Adobe system administrators manage user provisioning and entitlements for both products in the Adobe Admin Console.

Workfront Proof provides these additional user roles:

* **Proof Owner** manages the entire proof lifecycle, including assigning deadlines, reviewers, and permissions.
* **Observer** can view proofs but cannot comment or participate in reviews.
* **Workflow template manager** designs and manages reusable approval workflows.
* **Legal/Compliance Reviewer** reviews content for legal and regulatory compliance and has limited permissions.

No GenStudio for Performance Marketing roles map to these Workfront Proof roles.

### Approval templates

Workfront Proof approval templates provide preformatted workflow steps that can be quickly applied to a proof. These templates include predefined reviewers and approvers, proof roles, and deadlines, ensuring consistency and efficiency. Content creators launching a review can select from a set of predefined templates to apply the appropriate approval chain automatically, supporting both single-phase and multi-phase approval processes. Each stage of the workflow automatically associates the relevant reviewers, and all status updates and comments from the Workfront Proof workflow are visible within the Project Execution Module (PEM), enhancing transparency and collaboration.

### Comments

Comments can added and viewed 


### Version control

Workfront Proof enables digital review and approval of content through an interactive proof viewer, where each submission in the workflow represents a distinct version of the content. These versions are saved and can be compared side-by-side, allowing stakeholders to track changes and provide feedback efficiently. The system maintains a persistent history of all comments, decisions, and versions, supporting audit and compliance needs. Each version supports multi-stage, role-based approval workflows, with all approvals and rejections logged and timestamped. This structured versioning ensures transparency, accountability, and streamlined collaboration throughout the content lifecycle.

## Proof lifecycle
