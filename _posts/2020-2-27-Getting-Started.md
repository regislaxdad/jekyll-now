---
layout: post
title: Getting Started on GitHub Enterprise
---

## • Create and Setup User’s GitHub Account
	For more info about GitHub Enterprise, check this out: 
        https://niketechnology.slack.com/files/U0XU64QLU/F4G7N3ARE/welcome-to-github.pdf (Obsolete)

1. Go to Slack channel #baat-selfservice

2. Issue command: /github-access [NTuserID]  or  /github-access [user-email-addr]

   This will create the user’s account on Nike’s GitHub Enterprise. Essentially this step will add the user to the Active Directory group that is used by the GitHub Enterprise application when authenticating a user’s access to the platform.

3.  Go to https://github.nike.com to get logged in and to complete the account creation process. Essentially, upon successful login process, the user’s account on Nike’s GitHub Enterprise is established.

4.  Set up SSH key

       In the user’s personal settings on GitHub Enterprise, select “SSH and GPG Keys” section and click “New SSH key” to add the user’s SSH key, which is found in the user’s local desktop. This would allow the user the ability to clone a repository down to his/her local machine.
Enter an appropriate title and paste the “ssh-rsa” key then click “Add SSH Key”.

 
5. Request membership to appropriate Fusion Engineering team

   Contact Fusion Platform Operations team (via ServiceNow)
   Specify type of access or role: engineer, Lead, Gatekeeper/Approver
   Specify type of OSB services: nike, converse, soa, platform

6. Getting Familiar with Fusion OSB Organizations
	fusion-osb-production – organization for Fusion OSB repositories, teams and members representing the Fusion production environment
	fusion-osb-integration – organization for Fusion OSB repositories, teams and member representing the Fusion non-production environment, such as stage, qa and dev

7. Getting Familiar with Fusion OSB Repositories within Organizations

  * osb-services
  * java-services
  * osb-resources
  * osb-common-services
  * gateway-services
  * gateway-resources
  * soa-composites
  * osb-landscape-[landscape-name]


8. Download a Git or GitHub client
  * GitHub Desktop
  * Git Bash
  * On local machine, configure user’s GitHub userID and Nike email address:

    `git config --global user.name “<GitHub userId>”`

    `git config –global user.email “<Nike email address>”`

    `git config --list`
