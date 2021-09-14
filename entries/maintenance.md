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

About once a month, DLF MAWG website subgroup members will review the appropriate site(s), update ruby gems, and implement minor corrections or updates.

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

<h3>Deleting Branches</h3>

During the annual review process, DLF MAWG website subgroup members will need to delete branches, particularly merged and [**stale branches**](https://docs.github.com/en/github/administering-a-repository/managing-branches-in-your-repository/viewing-branches-in-your-repository).

To delete branches:

1. Open a browser and navigate to the appropriate original or forked repository.

2. Selecting ```branches```.

3. Selecting ```Stale```.

4. Clicking the trashcan icon next to any branch listed as ```merged```.

5. Repeat as necessary.

	- *Note*: If a branch is more than one year old, but has not been merged, consult with a maintenance team member to determine if the branch needs to be deleted.

<h3>Updating Ruby Gems</h3>

Periodically, your Ruby Gems will need to be updated. To do this:

1. Open a command line interface window.

2. Navigate to where your GemFile is located (e.g. the folder containing your local repository). 

3. Run the ```bundle update``` command.