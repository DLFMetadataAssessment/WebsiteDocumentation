---
sectionid: maintenance
layout: page
title: Maintaining the Repository
permalink: maintenance
---

{::options parse_block_html="true" /}

<h2>Introduction</h2>

This page describes the several maintenance workflows that members of the DLF MAWG website group employ to maintain the DLF MAWG's GitHub repositories. It also contains related information that should be useful in maintaining the DLF MAWG's sites.

<h2>Maintenance Team Members: Contact Information (2021-2022)</h2>

Maintenance members are responsible for answering questions and resolving issues. If you have questions, comments, or concerns about the documentation on this site, please don't hesitate to contact one of the following:

- Kate Flynn (kef@chicagocollections.org). 

- Steven Gentry (gentrysteven0208@gmail.com). 

<h2>Maintenance Workflows</h2>

<h3>Regular Review</h3>

About once a month, DLF MAWG website subgroup members will review the appropriate GitHub repositories, update ruby gems, and implement minor corrections or updates.

If the correction or update is significant--in other words, it substantially changes one or more pages--suggest it to a maintenance team member. They will make sure it is discussed during the next DLF MAWG website subgroup meeting.

<h3>Annual Review</h3>

Once a year, starting in July, the DLF MAWG website subgroup will conduct a review of its website to ensure the site is up-to-date in time for DLF Forum in the fall. This work involves:

- Reaching out to other subgroups to check that all information about their subgroup is correct.

- Collecting information about any project updates.

- Creating new pages for any new projects.

- Reviewing all relevant website pages for content issues (e.g. typographical errors) or access issues (e.g. missing or dead links).

- Updating any READMES as well as cleaning up each repository's branches.

- Resolving any outstanding issues for any relevant repositories. 

- Reviewing and updating our documentation.

<h3>Creating Collections</h3>

TBD.

<h3>Deleting Branches (Forks)</h3>

During the annual review process, DLF MAWG website subgroup members will need to delete branches, particularly merged and [stale branches](https://docs.github.com/en/github/administering-a-repository/managing-branches-in-your-repository/viewing-branches-in-your-repository) in your fork.

Delete branches on your fork by:

1. Open a browser and navigate to the appropriate original or forked repository.

2. Clicking ```branches```.

3. Clicking ```Stale```.

4. Clicking the trashcan icon next to any branch listed as ```merged```.

5. Repeat as necessary.

	- *Note*: If a branch is more than one year old, but has not been merged, consult with a maintenance team member to determine if the branch needs to be deleted.
	
During this time, maintainers should also delete any stale and outdated local branches and encourage site contributors to do the same. Delete local branches by:

1. Opening a command line interface tool and navigating to the folder on your computer containing your local copy.

2. Typing ```git branch``` to bring up a list of local branches.

3. Typing ```git branch -d BRANCHNAME``` to delete that the specific BRANCHNAME.

4. Repeating as necessary for each branch. 

<h3>Reverting Pull Requests</h3>

In the event that a pull request is erroneously merged into the default branch, immediately revert that pull request by:

1. Navigating to appropriate original repository in GitHub.

2. Clicking ```Pull Requests```.

3. Clicking  ```Closed```.

4. Clicking the appropriate closed pull request.

5. Clicking ```revert``` and approving the new pull request.

<h3>Updating Ruby Gems</h3>

Periodically, your Ruby Gems will need to be updated. To do this:

1. Open a command line interface tool of your choosing.

2. Navigate to where your GemFile is located (e.g. the folder containing your local repository). 

3. Run the ```bundle update``` command.