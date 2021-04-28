---
layout: page
title: Admin Best Practices
permalink: admin-best-practices
---
This documentation contains a set of recommended best practices for using Github inside of the University of Colorado Enterprise agreement.

Within your organization, everything is up to the administrating campuses' discretion. The following are recommendations, there is no policy in place that requires any campus to configure their Github organization in any way.

The following sections reflect the tabs available under 'Settings' for the organization you manage. Not all tabs will be covered, and once again these are only recomendations.

## Organization security
It is recommended that 'Require SAML SSO authentication for all members' is checked early in the configuration of the organization. Note that this DOES NOT stop ['outside collaborators'](https://docs.github.com/en/organizations/managing-access-to-your-organizations-repositories/adding-outside-collaborators-to-repositories-in-your-organization) from working on repositories, it simply means that anyone associated with the organization MUST use SSO to access resources in the organization. If you do not check this option any github user can be invited to be part of the organization and it will become difficult in the future to disambiguate who is actually part of the campus and who has just been invited in. However, again, that decision is left up to the campus, this is simply a recommendation.

## Member privileges
It is strongly recommended that under the 'Member Privileges' tab of 'Account Settings' for the organization that you set the 'Base permissions' to 'None'. Any other setting will allow any member of the organization to read any other repository in the organization. With this set to 'None', teams which control the repositories can allow access to their repositories on a user by user basis.

## Security & analysis
It is recommended to enable the following:
- Dependency graph
- Dependabot alerts
- Dependabot security updates

As mentioned at the bottom of the 'Security & analysis' tab, granting this access to private repositories is a bit trickier, that will be left up to the discretion of the admin.

## Verified domains
If you wish to take the [extra step](https://docs.github.com/en/organizations/managing-organization-settings/verifying-your-organizations-domain) you can get the 'verified' badge. This may reassure users that code is in fact coming from the actual university campus.