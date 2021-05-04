---
layout: page
title: Bitbucket to GitHub
permalink: end-user-faq
---
Moving your code from Bitbucket to Github is a fairly straightforward process. However, be aware that Bitbucket metadata, such as PR discussions will not move with your code. You will simply get your code along with the entire history and nothing more.

## An Opportunity for Change
Though we don't like to burden folks by making them move, change does happen, and with the Bitbucket to GitHub change, there is good opportunity to make further changes and review where you came from.
### Remove unneeded branches
Take a look at all the branches your repository currently has, are they all needed? If not consider removing stale branches before you move.
### Are there secrets in there?
Perhaps your code contained passwords at one time and you have since moved to something like HashiCorp's Vault, or AWS' Secrets Manager? If so perhaps it is time to consider whether you need the entire history of your code. The Platform Engineering team at CU Boulder took the admitadly radical step of just removing all of our code history before moving it over to GitHub. Each repo we created in GitHub had our up to date code, but only one commit, the initial commit. The steps needed for this are potenitally dangerous and are, as such, left up to the reader to determine.
### Be more inclusive
An easy step is to rename your 'main' branch from master to main, you can do this while [still using Bitbucket](https://dev.to/rhymu8354/git-renaming-the-master-branch-137b), you can do this during the move, or you can do this [after you are on Github](https://github.com/github/renaming).

## Creating an exact replica of your bitbucket repository on GitHub:
The following should get you an exact replica of your old repository on GitHub including all tags, branches, etc. this will NOT rename your main branch if it is already called master, it will still be called master after the move.
1. [Create the new repository](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-new-repository), choosing a name is up to you, but it is recommended that you prefix the repository with your groups name, for example oit-pe-example-repo.
1. git clone --bare https://bitbucket.host/old-repository.git
1. cd old-repository
1. git push --mirror https://github.com/CampusOrg/new-repository.git
1. cd ..
1. rm -rf old-repository