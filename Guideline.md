
## Guidelines for Git and GitHub use on Windows (For other OS, most of the guidelines are same) 

* Refer to GitAndGitHub_UserDocument.docx for Git and GitHub jargons, command reference, installation and configuration best practices.
* Install the latest version of Git (current 2.26.2 as of 20th April) for consistent behaviour of commands
* Follow coding guidelines for a cleaner code. E.g. consistent notations (like Camel or Hungarian notation), no whitespaces in documents
* Use master branch for stable code. 
* Feature development/bug fixing should be done on a separate (topic/feature) branch when working in a team and not directly on master branch
* The source of this feature branch should be merged with master branch.
* Rebasing should not be done for remote branches. (It will cause inconvenience to the other users use use your soure as baseline for dev)
* Avoid rebase for local branches too. The minor benefit of linear commits is not signification.
* Always work on a separate branch for a new development or fixing a bug.
* Have a basic set of test cases to check that no existing functionality breaks after any major commit (and minor too if necessary).
* Make use of tags/release labels once any milestone is achieved for the project
* Commit each feature separately as a logical set not as one massive code after many days. 
* Use staging area of Git to split source into different logical parts
* Each commit should have a descriptive (under 50 words), self-explanatory commit message. This will be useful when one refers to their source after many days
* Use 'Issues' function of GitHub, which provides milestones, issue classication and other features, to track new development and to log issues.
  When closing the issue associate it with a commit id for easy tracking of issue with commitid. 
  E.g. Use Issue id in commit message to close an issue. 
  close #4 at the end of a commit message. Or use a message as Associating #3 with the issue. This 
* Do not include files generated at runtime (e.g. binraries, log files, etc.) in repo. Use .gitignore file for the same
* Use commandline method to use Git and GitHub instead of GUI.
* Avoid modifying files directly on GitHub
* Keep version control versino of all source developed on GitHub for security, instead of keepign it only on local PC
* Make use of Markdown in comments on GitHub
* Readme.md markdown file is necessary in the root folder of the project as GitHub renders the Readme.md file when a user visits the directory showing its contents.
* Use SSH for cloning instead of https if promted for password at every push/pull
* Use Release GitHub feature to release your code at milestones (It can be created directly from GitHub)
* Use Gists to share a code snippet instead of Slack, if record of the share is to be kept for future reference.

## Recommended development steps when working in a team
1. git pull: Get latest master code
1. git branch *new_branchname*: Create branch
1. Make changes to the branch
1. Commit the changes to the branch
1. git push: To update the remote branch
1. Create Pull request on Github for code review
1. After review, merge the branch to master on GitHub
1. Delete remote branch *new_branchname*
1. Delete local branch *new_branchname*

## Working steps that can be used when working alone
Even though direct commit to master branch can be done, it is still recommended to follow above steps i.e. use a separate branch for development

