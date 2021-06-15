---
sectionid: contributing-to-site
layout: page
title: Contributing to the Website
permalink: doc/contributing-to-site
---

{::options parse_block_html="true" /}

# Introduction

Now that you have installed all necessary dependencies as well as configured your repositories, you are ready to begin contributing changes to the DLF website!

To facilitate contributing to the DLF MetadataAssessment repositories, we have provided two similar workflows:

- The first workflow primarily avoids the command line, and is envisioned as appropriate for those entirely new to Git and GitHub.

- The second workflow employs more of the command line. **We recommend using the second workflow once you become more familiar with Git, GitHub, and the GitHub workflow.**

# High Level Workflow

Regardless of which workflow you use, the general workflow for contributing changes is as follows:

1. Navigate to the appropriate original repository and review the issue you want to change.
2. Update your fork.
3. Update your local repository.
4. Use a text editor to effect changes.
5. Testing that the issue has been resolved.
6. Create a new branch.
7. Push the changed content into that new branch.
8. Create a pull request to merge the proposed changes into the original repository.
9. Assign reviewers.

Once you have contributed changes, the following workflow will be used to incorporate those changes into the original repository:

1. Review the change.
2. Merging the pull request and deleting the branch.

# Instructions for Contributing Changes (Minimal Command Line) 

1. Navigate to the appropriate original repository (e.g. the Sandbox) and review the issue you want to resolve.

	- **Note**: If you are not assigned to this issue, select **assign yourself** under **Assignees**.
	
	- **Note**: Review this video from Kate Flynn (from the time the video starts until 4:51) to learn more about how to review an issue: https://youtu.be/3fqsS2_ahXM?t=114

2. Ensure your fork is in sync with the original repository by:

	- Navigating to your fork.
	
	- Selecting the default branch (i.e. **main**).
	
	- Selecting **Fetch Upstream**.
	
	- (Optionally) Select **Compare** and review.
	
	- Selecting **Fetch and Merge**.

3. Ensure your local repository is in sync with your fork by:

	- Opening a terminal.
	
	- Navigating to folder on your computer containing your local repository, and further navigate into the folder containing the **README file.**

	- Ensuring you are on the default branch by typing the following into the terminal: **git checkout DEFAULT BRANCH NAME**. 
		
		- The DLF MAWG's default branch name is **main**.
		
	- Typing and entiering **gill pull origin DEFAULT BRANCH NAME**.
		
	- If you encounter a message like **Your branch is up to date with 'origin/DEFAULT BRANCH NAME'** then proceed to the next step. 
	
4. Using a text editor of your choice, and using the notes and information in the issue, **fix the issue in your local repository.**

5. Testing that the issue has been resolved. **For repositories that use Jekyll**, this will involve:
	
	- Navigating to your terminal, which should still be opened to local repository.
	
	- Running **bundle exec jekyll serve** to start Jekyll.
	
	- Navigating to the provided **Server Address** (e.g. http://127.0.0.1:4000) and reviewing the change.

6. Once you're ready so implement the change, select or create the branch that will house that change:
	
	- Navigate to your **fork**.
	
	- Select the branch drop-down menu and type the name of your branch into the search bar:
		
		- If you have already created a branch for this change, type that branch name into the search bar and select it.
		
		- If you need to create a new branch, type the name of the branch into the search bar and select the **create branch** option.
			
			- **NOTE**: Our branch naming convention is **issue#** followed by a four character number that represents the issue number. So, for a branch that resolves issue 189, the branch name would be issue#0189. 
		
7. Update the branch by:

	- Navigating to the **appropriate directory** in the fork. For example, if you changed a file that was in the **entries** sub-folder, make sure you select that sub-folder before proceeding to the next step.
	
	- Selecting **Add file** and then **Upload files.**
	
	- Dragging and dropping the changed file(s) from your local repository to the **Drag additional files here...** bar.
	
	- Scrolling to the bottom of the page, adding a title to your change (such as **Fixes issue#0189**) and any relevant descriptive information (such as **This also resolves a similar typographical issue in the breadcrumb**).
	
	- Selecting **Commit directly to the BRANCH NAME branch**.
	
8. Create a pull request to merge the content on the branch in your fork with the original repository:

	- Navigate to the main page of your fork.
	
	- Select the **Compare & Pull Request** button for the branch you just made.
	
	- If not already selected, click **Compare across forks**. 
	
	- Make sure that:
		
		- The **Base repository** is the original repository (e.g. DLFMetadataAssessment/Sandbox).
		
		- The **base** branch is the default branch (e.g. **main**).

		- The **Head Repository** is your fork.
		
		- The **compare** branch is the branch on your repository is the branch on your fork with the changed files. 
	
	- Review the title and description of the change and select **Create Pull Request**
	
9. Because no one is supposed to merge their own pull request into the original repository, complete this workflow by assigning a reviewer:

	- Selecting **Reviewers**.
	
	- Clicking on the search bar and selecting the name of the member you want to review this change.
	
# Instructions for Contributing Changes (More Command Line) 

1. Navigate to the appropriate original repository (e.g. the Sandbox) and review the issue you want to resolve.

	- **Note**: If you are not assigned to this issue, select **assign yourself** under **Assignees**.
	
	- **Note**: Review this video from Kate Flynn (from the time the video starts until 4:51) to learn more about how to review an issue: https://youtu.be/3fqsS2_ahXM?t=114

2. Ensure your fork is in sync with the original repository by:

	- Navigating to your fork.
	
	- Selecting the default branch (i.e. **main**).
	
	- Selecting **Fetch Upstream**.
	
	- (Optionally) Select **Compare** and review.
	
	- Selecting **Fetch and Merge**.

3. Ensure your local repository is in sync with your fork by:

	- Opening a terminal.
	
	- Navigating to folder on your computer containing your local repository, and further navigate into the folder containing the **README file.**

	- Ensuring you are on the default branch by typing and entering the following into the terminal: **git checkout DEFAULT BRANCH NAME**. 
		
		- The DLF MAWG's default branch name is **main**.
		
	- Typing and entiering **gill pull origin DEFAULT BRANCH NAME**.
	
	- If you encounter a message like **Your branch is up to date with 'origin/DEFAULT BRANCH NAME'** then proceed to the next step. 
	
4. Using a text editor of your choice, and using the notes and information in the issue, **fix the issue in your local repository.**

5. Testing that the issue has been resolved. **For repositories that use Jekyll**, this will involve:
	
	- Navigating to your terminal, which should still be opened to local repository.
	
	- Typing and entering **bundle exec jekyll serve** to start Jekyll.
	
	- Navigating to the provided **Server Address** (e.g. http://127.0.0.1:4000) and reviewing the change.

6. Once you're ready so implement the change:

	- Navigating to the your terminal.
	
	- Terminate the server by typing and entering **y** until it closes.
	
	- Typing **git checkout -b BRANCHNAME** to create a new local branch in your repository and switch to that branch.

		- **NOTE**: Our branch naming convention is **issue#** followed by a four character number that represents the issue number. So, for a branch that resolves issue 189, the branch name would be issue#0189. 
		
7. Update the branch by:

	- Navigating to the your terminal.

	- Typing and entering ** git add** and the file paths of the fikles that you changed.
		
		-**NOTE**: You can either add individual files or add all changed files. To add a certain number files, we recommend using the **Copy as path** method to  for each file. Otherwise, simply type and enter **git add .** to add all changed files.
	
	- Typing and entering **git commit -m "fixes issue#NUMBER",** where NUMBER is the issue number. This will add an explanatory note to your commit.  
	
	- Typing and entering **git push --set-upstream origin issue#NUMBER** (use the same branch name as in the previous step). This branch from your local repository should now be on your fork. 
	
	- Finally, type and enter **git checkout DEFAULT BRANCH NAME** to return to the default branch.
	
8. Create a pull request to merge the content on the branch in your fork with the original repository:

	- Navigate to the main page of your fork.
	
	- Select the **Compare & Pull Request** button for the branch you just made.
	
	- If not already selected, click **Compare across forks**. 
	
	- Make sure that:
		
		- The **Base repository** is the original repository (e.g. DLFMetadataAssessment/Sandbox).
		
		- The **base** branch is the default branch (e.g. **main**).

		- The **Head Repository** is your fork.
		
		- The **compare** branch is the branch on your repository is the branch on your fork with the changed files. 
	
	- Review the title and description of the change--and add any additional description you feel is necessary--and select **Create Pull Request**
	
9. Because no one is supposed to merge their own pull request into the original repository, complete this workflow by assigning a reviewer:

	- Selecting **Reviewers**.
	
	- Clicking on the search bar and selecting the name of the member you want to review this change.	

# Reviewing and Approving Changes
	
1. Once you have been assigned to a change, review the change by:
	
	- Reviewing the title and description of the pull request and comparing it to the original issue, to ensure the actual issue was nominally addressed.
	
	- Reviewing the **Files Changed** tab to confirm that the change was actually implemented.
	
	- Checking to ensure there are no branch conflicts.
		
		- **Note**: If there are branch conflicts, please reach out the DLF MAWG group members listed in the [Maintenance](maintenance) page to resolve this issue.
		
2. Once you are satisfied this change is sufficient, merge the branch into the original repository by:

	- Clicking the **Merge Pull Request** drop-down arrow and ensuring that **Create a Merge Commit** is selected.

	- Selecting **Merge pull request**. 
	
	- Deleting the merged branch.