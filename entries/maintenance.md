---
sectionid: maintenance
layout: page
title: Maintaining the Repository
permalink: maintenance
---

{::options parse_block_html="true" /}

<h2>Introduction</h2>

This page describes several maintenance workflows that members of the DLF MAWG website group employ to maintain the DLF MAWG's GitHub repositories. It also contains related information that should be useful in maintaining the DLF MAWG's repositories.

<h2>Maintenance Team Members: Contact Information (2021-2022)</h2>

The following maintainers are responsible for answering various questions and resolving issues related to any of DLF MAWG's repositories (including this documentation site):

- Kate Flynn (kef@chicagocollections.org). 

- Steven Gentry (gentrysteven0208@gmail.com). 

<h2>Maintenance Workflows</h2>

<h2>Regular Review</h2>

About once a month, DLF MAWG website subgroup members will review one or more appropriate GitHub repositories, update ruby gems, and implement minor corrections or updates.

If the correction or update is significant--in other words, if the correction or change would substantially change one or more pages--we ask that you reach out to one of the above maintainers/maintenaince member. They will make sure it is discussed at the next DLF MAWG website subgroup meeting.

<h2>Annual Review</h2>

Once a year, starting in July, the DLF MAWG website subgroup will conduct a review of its primary website and repository to ensure that the site and repository is up-to-date in time for DLF Forum in the fall. This work involves:

- Reaching out to other subgroups to check that all information about their particular subgroup is correct.

- Collecting information about any particular project updates.

- Creating new pages for any new projects.

- Reviewing all relevant website pages for content issues (e.g. typographical errors) or access issues (e.g. missing or dead links).

- Updating any READMES as well as cleaning up each repository's branches.

- Resolving any outstanding issues for any relevant repositories. 

- Reviewing and updating our documentation.

<h2>Creating Collections</h2>

TBD.

<h2>Deleting Branches</h2>

During the annual review process, DLF MAWG website subgroup members will need to delete branches, particularly merged and [**stale branches**](https://docs.github.com/en/github/administering-a-repository/managing-branches-in-your-repository/viewing-branches-in-your-repository) in your fork.

Delete branches on your fork by:

1. Opening a browser and navigating to the appropriate repository.

2. Clicking **branches**.

3. Clicking **Stale**.

4. Clicking the trashcan icon next to any branch listed as **merged**.

5. Repeat as necessary. 

If a branch is more than one year old, but has not been merged, consult with a maintenance team member to determine if the branch needs to be deleted.
	
During this time, maintainers should also delete any stale and outdated local branches and encourage site contributors to do the same. Delete local branches by:

1. Opening a command line interface tool and navigating to the folder on your computer containing your local copy.

2. Typing ```git branch``` to bring up a list of local branch names.

3. Typing and entering ```git branch -d``` *and one of the names of a local branch that appeared in the previous step.* This will delete that specific branch.

4. Repeating as necessary for each branch that you want to delete. 

<h2>Updating Ruby Gems</h2>

Periodically, your Ruby Gems will need to be updated. To do this:

1. Open a command line interface tool of your choosing.

2. Navigate to where your GemFile is located (e.g. *the folder containing your local repository*). 

3. Type and enter ```bundle update```.