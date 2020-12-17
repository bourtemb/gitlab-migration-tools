# tango-controls is moving from Github to Gitlab

## Context
The Tango Steering Committee took the decision to move the tango-controls git repositories from Github (https://github.com/tango-controls) to Gitlab (https://gitlab.com/tango-controls).
This decision was taken as a consequence of the recent changes in Travis CI policy which will no longer be as Open Source Software friendly as in the past, starting from january 1st 2021. 
Open Source projects like tango-controls are now considered as sponsored projects and no longer benefit from the same advantages as before.
So it has been decided to replace Travis CI with an alternative.
Since most of the institutes using tango-controls are already using gitlab for their private projects and gitlab-ci is a good alternative to travis CI, 
it has been decided to migrate the tango-controls github repositories to Gitlab.
The repositories migration should not be too complicated since Gitlab provides an import tool able to import the most important things from Github (issues, wiki, etc..).
The issue numbers will be preserved.

tango-controls got granted a free gitlab.com gold license (for 100 seats), since it is an Open Source project.

## Migration
In general, you can follow and comment the migration process on https://github.com/tango-controls/TangoTickets/issues/44 issue.

The migration from Github to Gitlab will focus primarily on the most active projects currently using Travis CI (like cppTango, pytango, jtango, TangoSourceDistribution).

The projects will be migrated one by one by the tango-controls Gitlab migration team in coordination with the different tango-controls Github repositories administrators.

To ensure a smooth migration, it is important/better that the contributors of all the migrated repositories (commits, comments on issues or pull requests, issue creators) 
connect once on gitlab.com using the Github authentication AT LEAST 24 HOURS BEFORE THE MIGRATION. 
Another possibility is for these users to create an account on gitlab.com AT LEAST 24 HOURS BEFORE THE MIGRATION using the same e-mail address as their Github primary address which MUST BE PUBLIC in this case.
Please note that if you set up Github to keep your e-mail address private, all the commits done with an address like my-github-account@noreply.github.com will not be recognized as coming from your gitlab or gthub account. So your contribution stats might not be as good as before for your past contributions.

If a contributor does not login on gitlab.com using the github button or if his e-mail addresses on his gitlab.com account do not match the PUBLIC e-mail addresses set on his Github account, all the comments made by this contributor will appear as created by the tango-controls-bot account.
A line will be added in the comment, specifying that this comment was originally created by <<the github user>>.

A migration dedicated issue will be created in each Github repository to coordinate the migration.
This issue will mention all the contributors of the project and inform them about the deadline to log in to Gitlab with their Github account or to create a gitlab.com account using the same e-mail address as their Github public primary address.

If you are using several e-mail addresses on Github (alternate e-mail addresses), it might be useful to specify them as well in you Gitlab account to ensure all your commits are correctly linked to your Gitlab account.

### Migration steps:
1- Convert the Travis CI yml file to an equivalent gitlab-ci yml file and test it on a test gitlab repository.
2- Decide with the repository admins on a date for the migration to Gitlab
3- Publish a deadline for the users to login to gitlab using the github authentication button or use the same e-mail address as the Github PUBLIC prmary address in the gitlab.com account.
4- The Tango-Controls Gitlab migration team (https://github.com/orgs/tango-controls/teams/gitlab-migration) will migrate the repository at least 24h after the login deadline (to ensure all the new accounts are well taken into account by Gitlab).
The migration will be done using the tango-controls-bot generic account.
Before the migration, the Github repository might be switched to archive mode (read-only) to ensure no modification occurs during the migration.

The repositories on github will probably be kept as read-only mirrors of the gitlab repositories.


