---
layout: article
title: Proof-of-Concept Project Checklist
categories: [business]
featured: false
popular: false
hidden: false
tags: [project guide, poc]
order: "05"
redirect_from:
  - /bitwarden-proof-of-concept-project-guide/
---

This guide is designed by our Product, Implementation, and Sales specialists at Bitwarden to help guide your business in running a PoC of Bitwarden. Bitwarden offers a free trial for [Enterprise Organizations](/about-organizations/), and we're confident that spreading out these steps over that time will help shape a successful PoC.

|Day|Action|Key Person|Description|Resource(s)|Duration (hrs)|
|:-:|:----:|:--------:|:---------:|:---------:|:------------:|
|1|Identify an Organization Owner|Organization Owner|[Create a free Bitwarden account](https://vault.bitwarden.com/#/register){:target="\_blank"} for your Organization Owner, who will manage your Organization's settings, structure, and subscription.|[Create your Bitwarden Account](/create-bitwarden-account/)|0.1|
|1|Create your Organization|Organization Owner|[Create a **free Organization** on the Bitwarden Cloud](/getting-started-organizations/#setup-your-organization). Once created, let us know and we'll upgrade you to an Enterprise trial.<br><br>If you're self-hosting, this Organization will be used only for billing purposes.|[Organizations](/about-organizations/)|0.1|
|1|(**Self-hosting only**) Download a License|Organization Owner|If you're self-hosting Bitwarden, a license file enables Enterprise functionality and the right number of seats for your instance.|[License Paid Features](/licensing-on-premise/#organization-license)|0.1|
|1|(**Self-hosting only**) Install Bitwarden|Organization Owner / IT Team|Setup your Bitwarden server. We recommend deploying on Linux for optimal performance and lowest total cost of ownership.|[Install and Deploy](/install-on-premise/)|2.5|
|1|Add Admins|Organization Owners + Admins|Onboard [Admins](/user-types-access-control/) to Bitwarden, who can manage *most* Organization structures. We also recommend adding a second Owner for redundancy.|[User Management](/managing-users/)|0.2|
|2|Create Collections|Organization Owners + Admins|Create [Collections](/about-collections/), which gather items for secure sharing with Groups of users.|[Collections](/about-collections/)|0.25|
|2| Create Groups|Organization Owners + Admins|Create [Groups](/about-groups), which gather users for scalable assignment of permissions and access to Collections.<br><br>If you decide to sync Groups and users from your Identity Provider or Directory Service, you may need to reconfigure user and Group assignments later.|[Groups](/groups/)|0.25|    
|2|Assign Groups to Collections|Organization Owners + Admins| Assign Groups to Collections, making shared items available to supersets of users. Test the *Read Only* and *Hide Password* options.|[Collections Assignment](/about-groups/#edit-collections-assignments)|.5|
|2|Share items to Collections|Organization Owners + Admins|[Add items manually](/sharing/#create-an-organization-item) or [import data](/import-to-org/) from another password management application.|[Sharing](/sharing)<br><br>[Import to an Organization](/import-to-org/)|0.25|
|2|Configure Enterprise Policies|Organization Owners + Admins|Enterprise Policies can be used to tailor your Bitwarden Organization to fit your security needs. **Enable and configure desired policies before user onboarding begins.**|[Enterprise Policies](/policies/)|0.1|
|3|Add users to Groups|Organization Owners + Admins|Add a set of users to your Organization manually and assign them to different groups. With these users, you'll broadly test all pre-configured functionality **in the next step**, before moving on to advanced functions like Directory Connector.|[User Management](/managing-users/)<br><br>[Groups](/about-groups/)|0.5|
|3|Download Bitwarden Client Applications|All users|All Organization members should download Bitwarden on an assortment of devices, login, and test access to shared items/Collections/Groups and application of applied Policies. **If you're self-hosting,** users will need to [connect each client to your server](/change-client-environment).|[Download Bitwarden](https://get.bitwarden.com/)|0.5|
|4-6|Configure Login with SSO|Organization Owners + Admins|Configure Bitwarden to authenticate using your SAML 2.0 or OIDC Identity Provider.|[About Login with SSO](/about-sso/)|1.5|
|4-6|Configure and test user onboarding with Directory Connector|Organization Owners + Admins|Download, configure, and test the Bitwarden Directory Connector application, which is used to automatically sync users and groups from your existing directory service (LDAP, AD, etc.)|[About Directory Connector](/directory-sync/)|1.5|
|4-6|Configure Directory Connector for production onboarding|Organization Owners + Admins|Execute on using Directory Connector to invite your remaining users to the Organization.|[Directory Connector Desktop App](/directory-sync-desktop/)|1|

## Deployment Best Practices

We've seen a lot of deployments and have found that taking the following actions can positive contribute towards a successful PoC and successful adoption with your users:

|Day|Action|Key Person|Description|Resource(s)|Duration (hrs)|
|:-:|:----:|:--------:|:---------:|:---------:|:------------:|
|4-6|Determine timeline for rollout to first-wave users|Senior Leadership & Security teams|There are lots of different strategies for rolling out Bitwarden. Take things at whatever pace best suits your team.| | |
|7|Craft internal messaging about Bitwarden rollout|Internal Training & Managers|Bitwarden provides a lot of resources to help users quickly adopt, check some out on [Youtube](http://youtube.com/bitwarden) and on the [Help Center](https://bitwarden.com/help/).|[Youtube](http://youtube.com/bitwarden)<br><br>[Help Center](https://bitwarden.com/help/)||  
|7|Communicate to internal leaders about Password Management policies|Internal leaders / Security teams|Make sure your teams know about any [Enterprise Policies](/policies), [2FA](/setup-two-step-login-duo/) or [SSO](/about-sso/) requirements, and password management best practices.| | |
| | | | | | |
| | | | |**Total Hours (Cloud-hosted)**|**7.35**|
| | | | |**Total Hours (Self-hosted)**|**9.85**|
