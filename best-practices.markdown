---
layout: page
title: Github Best Practices
permalink: best-practices
---
This documentation contains a set of recommended best practices for using Github inside of the CU Enterprise agreement.

## Teams
Use teams to organize your work. By default any private repository you create will not be accessible to anyone else in the organization. If you wish to collaborate with others, it is strongly recommended that you [create a team](https://docs.github.com/en/organizations/organizing-members-into-teams/about-teams).

## Github Actions Minutes
Github has the concept of [Github Actions](https://docs.github.com/en/actions/learn-github-actions) it is essentially a cloud based CI/CD system (Jenkins like). CU's license agreement with Github allows for 50,000 action minutes per month, after the limit is reached, no further actions will execute. Action minutes are only counted against private repositories, as such it is recommended, as much as is reasonable, to make your repositories public.

In addition, not all action minutes are created equal. If running actions on a MacOS system each wall minute counts as 10 action minutes, similarly for windows each wall minute counts as 2 action minutes, [more info here](https://docs.github.com/en/github/setting-up-and-managing-billing-and-payments-on-github/about-billing-for-github-actions). As such, please try to limit your Github Actions time to Linux based runners if at all possible.

## Security
Security of your code and your repositories is your responsibility, please avail yourself of the [Github Security documentation](https://docs.github.com/en/code-security/getting-started/about-securing-your-repository).