---
layout: page
title: Admin Best Practices
permalink: admin-best-practices
---
This documentation contains a set of recommended best practices for using Github inside of the University of Colorado Enterprise agreement.

Within your organization, everything is up to the administrating campuses' discretion. The following are recommendations, there is no policy in place that requires any campus to configure their Github organization in any way.

The following sections reflect the tabs available under 'Settings' for the organization you manage. Not all tabs will be covered, and once again these are only recomendations.

## Member privileges
It is strongly recommended that under the 'Member Privileges' tab of 'Account Settings' for the organization that you set the 'Base permissions' to 'None'. Any other setting will allow any member of the organization to read any other repository in the organization. With this set to 'None', teams which control the repositories can allow access to their repositories on a user by user basis.

## Security & analysis
It is recommended to enable the following:
- Dependency graph
- Dependabot alerts
- Dependabot security updates

As mentioned at the bottom of the 'Security & analysis' tab, granting this access to private repositories is a bit trickier, that will be left up to the discretion of the admin.

