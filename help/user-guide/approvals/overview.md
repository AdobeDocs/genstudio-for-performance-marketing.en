---
title: Adobe GenStudio for Performance Marketing Reviews and Approvals
description: Learn about the GenStudio for Performance Marketing review and approval process.
level: Beginner
feature: Content Review, Content Management
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
---
# Adobe GenStudio for Performance Marketing Reviews and Approvals

The review and approvals workflow ensures that all stakeholders— from creative teams to legal experts— can efficiently review and approve campaign assets and experiences, including generative AI-produced brand assets.

>[!NOTE]
>
> This feature is also available as an [integration with Adobe Workfront Proof](./proof-integration.md). This integration delivers Proof capabilities in the GenStudio for Performance Marketing Canvas. With the Workfront Proof integration, GenStudio for Performance Marketing gains a more structured, transparent, and collaborative review process, helping teams move from draft to final with greater confidence and clarity. 

## [!DNL Review and Approval] workflow advantages

* **Support for robust, iterative generative AI content creation**. Creating and deploying brand-aligned content in an organization is a highly iterative process. GenStudio for Performance Marketing generative AI capabilities support the quick creation of hundreds of asset variants. Each reviewer might request multiple changes to an asset draft before approving it. The more reviewers, the greater the number of potential iterations before all stakeholders agree on a final variant.

* **Support for creative integrity**. Approvals safeguard the creative integrity of your brand assets by keeping content creators involved in the approval process. By involving creative stakeholders (for example, content creators and creative directors) in the review and approval process, you ensure that final output aligns with your vision and brand identity.

* **Adherence to campaign goals and legal requirements**. The approval process helps verify that content supports campaign goals. It ensures that all marketing materials comply with legal and regulatory standards, which minimizes risks and potential legal issues.

* **Integration with Adobe Workfront Proof**. Users can access Workfront Proof's robust review-and-approval capabilities from within GenStudio for Performance Marketing. Content reviewed in GenStudio for Performance Marketing is synced to Workfront Proof, and review comments and status are preserved. [Integration highlights](./proof-integration.md) identifies how Proof extends GenStudio for Performance Marketing's approval workflow.

## Review and approval lifecycle

The main phases of the review and approval workflow include:

* [Request review and approval of content you have created](./request-review.md). GenStudio for Performance Marketing streamlines the process of requesting approvals and managing approvers. Workfront Proof approval templates can simplify this task even more.

* [Review and edit content](./review-and-edit.md). Notifications keep content creators in the loop about requested changes and approvals. Revising content triggers an automatic new approval cycle.

* [Approve content](./approve-content.md). Designated approvers mark content as approved, or ready for publication.

* [Publish content](./publish-content.md). Publishing approved content to [!DNL Content] makes it available for others in your organization to use or reference.

## About [!DNL Content] drafts

_Drafts_ are preliminary versions of assets or experiences that have not completed the review and approval process. Draft status identifies where the draft is in the review and approval process. A unique draft ID identifies each draft. This ID is valid until a draft is approved and published to [!DNL Content]. Review comments and approvals for a draft are associated with this individual draft ID. There is no versioning for GenStudio content drafts.

When a draft completes the review and approval process and is published to [!DNL Content], the draft ID expires. GenStudio for Performance Marketing does not save associated comments and approval status. The draft URL is no longer valid. 

Draft status captures the state of the content draft as it moves through the review and approval process. The GenStudio for Performance Marketing content editor who created the asset under review is notified of any requested changes to the draft or approvals. Approvers change draft status to indicate whether a draft needs further revision or can be approved. All designated approvers must approve an asset or experience before it can be published.

Available draft statuses:

**Notified**: Content editor has started the review and approval process by notifying approvers that a draft is ready for review.
**Needs work**: Indicates that one or more approvers has requested changes to the content draft. Content in this status cannot be saved to [!DNL Content].
**Approved**: All designated approvers have approved the asset or experience. The content editor can now add metadata to the asset or experience and save it to [!DNL Content].

>[!NOTE]
>
> Drafts correspond to _proofs_ for users of the Workfront Proof integration. [Proofs and drafts](proof-integration.md#drafts-and-proofs) differ in terms of persistence and versioning.

## Approval roles

_Reviewers_ can add comments but cannot approve content. Reviewer participation is helpful but not essential. _Approvers_ must approve content before it can progress through the approval process. Workfront Proof integration supports a wider range of user roles.


## Notifications

GenStudio for Performance Marketing in-product notifications update approvers and content editors in real time of asset status changes and `@mention` comments. Notifications support speedy iteration through the multiple review, edit, and approval cycles.

Content editors and approvers can sign up to receive these notifications in Slack. See [Subscribe to services in Experience Cloud](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences#slack).

Actions taken by approval participants trigger automatic in-product notifications and email notifications. When you start an approval process, designated approvers receive both email and in-product notifications. You are kept in the loop with in-product and email notifications whenever an approver adds `@mention` comments or makes a decision. Notifications include links to the content draft.

If you initiated the review and approval process for content, you are notified of all approvals and review comments. However, approvers are notified of only comments that include them with an `@mention`.
