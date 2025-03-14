---
title: Optimize your activation
description: Learn how to optimize activations to third-party paid ad channels.
---
# Optimize activations

Activating an ad experience for paid ad channels involves two main phases:

* Preparing your experience for activation

* Publishing your experience to its designated paid channel ad managers

Following best practices when creating and activating your ad experience can help minimize potential complications or errors during delivery to target channels.

## Best practices

Here are some common best practices and the errors that they can prevent.

* **Use valid, complete destination URLs**

Invalid URLs can trigger errors. Sample error: _The URL you entered doesn't direct to a website. Please enter a valid URL and try again. (100)_

* **Ensure that your application handles token expiration correctly**

Applications should request new tokens as needed. As needed, re-authenticate and obtain a new access token by logging in again or refreshing the session. Sample error: _Error validating access token: The session has been invalidated because the user changed their password or Facebook has changed the session for security reasons. (190)_

* **Review your ad set and ensure that only one ad is active at any time**

If you need to activate multiple Meta Ads, create a separate Dynamic Creative Ad Sets for each one. Sample error: _Dynamic Creative Ad Set allows at most one active ad in it. Users are not allowed to create more than one ads under the same Dynamic Creative Ad Set. (100)_

* **Match the number of applied rules with the amount specified by the platform**

Paid channels expect the number of applied rules to match their specified format.  If necessary, adjust the number of rules to match the value that the platform specifies. Sample error: _The Ad AssetFeed has X target rule(s) for format: name of format, but exactly X target rule for this format is expected. (100)_

* **Choose a call-to-action (CTA) that is compatible with your ad set objective**

Call-to-actions that are incompatible with the objective in Dynamic Creative Ad Sets trigger an error. Sample error: _The call to action type X is not supported for the objective Y in Dynamic Creative Ad Set. (100)_

* **Ensure the target ad set's cap supports the number of ad experiences**

Confirm the target ad set's ad limit can accommodate your activated ad experiences. If necessary, remove any unnecessary or inactive ads from the ad set to stay within this limit. Alternatively, create a new ad set to activate additional ads. Sample error: _You have reached the campaign, ad set or ad limits per Ad account. Each ad set can contain a maximum of 50 ads. This includes paused / inactive / turned off ads. (100)_

* **Ensure that the platform supports your selected CTA type**

Confirm that your experience includes a supported CTA type. Sample error: _(#100) Invalid call to action type (100)_
