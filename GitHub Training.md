# GitHub Training [slide 1]

* We will not be covering git or github basics - instead this is aimed at the enterprise and cloud-specific features that GitHub provides.

* We will cover what Enterprise adds to the GitHub product, I'll demo some features of GitHub like codespaces and actions, and then I hope to have some time for Q & A

## Authentication and Enterprise [slide 2]

* Organizations have repos and people [slide 3]

* Enterprise is a layer of icing on top. [slide 4]

* Joining an organization into the enterprise opens up shortcode billing for toll services, the ability to get GH Advanced Security, and support under our agreement.

* GH has a "bring your own identity" strategy. [slide 5]
  * Create your own GitHub account, just add a umich.edu address to it.
  * You can mix a personal account and university work in the same account, or
  * You can create a 2nd github account and keep them separate. [slide 6]

* By creating an organization in the "enterprise", users who are not specifically tagged as "outside collaborators" will lose access when they no longer have a university affiliation. You must sign in to WebLogin once every 7 days.

* There's no MCommunity or AD sync as GH's APIs are too limited (but, pending some changes from GH, it might happen). [slide 7]

## Codespaces [slide 8]

* So one of the best features of GitHub is Codespaces, which lets you bring up a VM to do work in without needing to run or install anything on your Mac.

* A lot of projects are touched infrequently once launched, and launching that specific combination of language, database, etc, is not easy.

* Getting new developers "working" can take a lot of time, and often burdens an expert while they are getting the newbie operational.

* I'm going to launch a new codespace for this simple project, and then I'm going to bring it into VSCode to work on it by clicking this button here. [slide 9]

* Now, let's make a quick edit to this file (edit something trivial, launch the app - show how other people can get to the preview of the app as well)

* In VSCode, the GitHub extension provides views into any issues and pull requests in my repo. I'm going to begin working on this issue by clicking the arrow button here, which creates a new branch for this issue.

* Let's make a quick change, save it, looks good - let's create a pull request.

## GitHub Actions

* GitHub Actions let you automate the software development and deployment steps. For example, this project has a GH Action that runs unit tests automatically against pull requests when the PR is updated.

* Here you can see that the PR unit test was successful, so merging is allowed.

* If the unit test failed, a contributer would need to update their code until the unit test succeeded.

* Once the merge to main is complete, another Action is run to deploy the finished product to our beta server. [ open the beta site]

* We have one more action associated, which updates the production website when a GitHub "release" is created. Let's go make a release here, describing what we changed. [create a release, watch it push to production]

* Actions can do more than just integration and deployment, they can also manage issues, pull requests, releases, and so on.

## Codespaces Part Two

* One of the compelling features of Codespaces is that GitHub provides an entire in-browser version of VSCode alongside the codespace. So you can work on your project from an iPad.

[ Flip to iPad ]

* So, I'm out of town, and my colleague tells me that their PR is broken.

* I launch a new Codespace just for that specific PR. This doesn't impact my previous codespace, which might have incomplete work in it.

* Ah here we are, there's a leftover debugging exception. I'll remove it, save that back to the PR, and commit it here.

##
