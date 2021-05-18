---
layout: page
title: GitHub Service Accounts
permalink: service-accounts
---
The definition of service accounts differ, but for the purposs of this document, a service account is any account that is not linked to a human. These are often used for automation tasks and the like.

GitHub handle single sign on (SSO) differently than most other providers, as such service accounts take a little bit of extra work to get running.

## Prequisites
1. A service account associated with the campus that controls the GitHub organization you wish to use as well as the associated password for that service account. As an example, for the Boulder campus to use the [UCBoulder](https://github.com/UCBoulder) organization, you would need a service account in [Boulder's identity provider](https://identikey.colorado.edu).

## Creating a Service Account in GitHub
1. [Creat a GitHub account](https://github.com/join).
1. Once logged into your new GitHub account, single sign on to the GitHub organization you wish to use using the service account you already had for your campus (note, the account names of your GitHub service account and your campus service account do not have to be identical). The two accounts are now associated.
1. Still signed in to GitHub with the service account, create a [personal access token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token), [SSH key(https://docs.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account)], [OAuth app](https://docs.github.com/en/github/authenticating-to-github/authorizing-oauth-apps) or whatever you need.
1. Ensure that the [personal access token](https://docs.github.com/en/github/authenticating-to-github/authorizing-a-personal-access-token-for-use-with-saml-single-sign-on), [SSH key](https://docs.github.com/en/github/authenticating-to-github/authorizing-an-ssh-key-for-use-with-saml-single-sign-on) are authorized with your campus' organization.

The GitHub service account should now have access to the organization you need and be configured for automation via a personal access token, an SSH key, or the like. 
