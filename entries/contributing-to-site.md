---
sectionid: contributing-to-site
layout: page
title: Contributing Changes
permalink: contributing-to-site
---

{::options parse_block_html="true" /}

<h2 id="top">Page Sections</h2>

<ul>
	<li><a href="#workflowhigh">High Level Workflow</a></li>
	<li><a href="#mincomline">Instructions for Contributing Changes (Minimal Command Line)</a></li>
	<li><a href="#morecomline">Instructions for Contributing Changes (More Command Line)</a></li>
	<li><a href="#revandappro">Reviewing and Approving Changes</a></li>
	<li><a href="#otherwork">Other Workflows</a></li>
</ul>

<h2 >Introduction</h2>

[**Now that you have installed all necessary dependencies, as well as configured your repositories**](installation), you are ready to begin contributing changes!

To facilitate contributing, we have provided two similar workflows:

- The first workflow primarily avoids using the command line and is envisioned as more appropriate for those who are fairly new to Git and GitHub.

- The second workflow employs more of the command line. 

We recommend using the second workflow once you are comfortable with the command line, Git, GitHub, and the GitHub workflow.

<h2 id="workflowhigh">High Level Workflow</h2>

Regardless of which specific workflow you use, the general steps are the same:

1. Navigate to the appropriate original repository and review the issue(s) that you want to address.

2. Update your fork.

3. Update your local repository.

4. Use a text editor to make changes in your clone.

5. Test your clone to ensure that you have resolved the issue(s).

6. Create a new branch to house your change.

7. Push the branch with these changes to your fork.

8. Create a pull request to merge the branch into the original repository.

9. Assign reviewers to review your pull request.

Once you have assigned one or more reviewer(s), those reviewers will:

1. Review the change.

2. Merge the pull request and delete the branch (if everything is satisfactory), or

3. Reach out to the change contributor to resolve the issue(s) before repeating the process outlined in step 2 (if further revisions are necessary).

<a href="#top">Return to top</a>

<h2 id="mincomline">Instructions for Contributing Changes (Minimal Command Line)</h2> 

1. Navigate to the appropriate original repository and review the issue you want to resolve.

	- NOTE: If you are not assigned to this issue, select **assign yourself** under **Assignees**.
	
	- NOTE: If an issue has not yet been created, contact a [**Maintenance**](maintenance) team member, who will create an issue for you.
	
	- NOTE: Review [**this video from Kate Flynn**](https://youtu.be/3fqsS2_ahXM) (from the time the video starts until 4:51) to learn more about how to review an issue.

2. Ensure that your fork is in sync with the original repository by:

	- Opening a browser and navigating to your fork.
	
	- Selecting the default branch if it is not already selected. Typically, this branch will be named **main**.
	
	- Selecting **Fetch Upstream**.
	
	- (Optionally) Select **Compare** and review.
	
	- Selecting **Fetch and Merge**.
	
3. Ensure your local repository is in sync with your fork by:

	- Opening a command line interface tool.
	
	- Navigating into the folder on your computer containing your local repository by typing and entering ```cd``` *and the name of the folder containing your clone*.

	- Navigating into the folder containing the README file using the same instructions as above.

	- Typing and entering the following into your command line tool: ```git checkout``` *and your clone's default branch name* (to make sure you are on the default branch).  The DLF MAWG's default branch name across all repositories is typically called **main**.

	- Typing and entering ```git pull origin``` *and your fork's default branch name* into your command line tool, which will pull and merge the material in your fork's default branch into your local repository.
		
	- NOTE: If you encounter a message like **Your branch is up to date with 'origin/DEFAULT BRANCH NAME** in your command line tool when you complete the final part of step 3, then proceed to the next step. 	
	
4. Fix the issue in your local repository by:

	- Navigating to the folder on your computer containing your local repository (see above for details regarding how to do this).
	
	- Opening the appropriate file(s) using the source code editor of your choice.
	
	- Making the appropriate change(s). 

5. Test that the issue has been resolved by:
	
	- Opening your command line interface tool, and--if necessary--navigating to the directory containing the README file of your clone (see above for details regarding how to do this).
	
	- Typing and entering ```bundle exec jekyll serve``` into your command line tool to start Jekyll locally on your computer.
	
	- Navigating to the provided **Server Address** (e.g. http://127.0.0.1:4000) and reviewing the change(s) that you made.
	
	- Terminating the server by navigating to your command line tool, holding **Ctrl-C**, and typing and entering ```y``` until the command line interface window notes that the server has closed.

6. Once you're ready so propose implementing the changes into the original repository, you will need to select or create the branch that will house the change(s). You can do this by:
	
	- Opening a browser of your choice and navigating to your fork.
	
	- Selecting the **branch drop-down menu**, typing the name of your branch into the **search bar**, and doing one of the following:
		
		- If you have already created a branch for this particular change, type that branch name into the **search bar** and select the branch.
		
		- If you need to create a new branch, type the name of the branch into the search bar and select the **create branch** option. Our branch naming convention is **issue#**, followed by a number that is the same as the issue number. For example, if the issue number is 200, the branch name would be **issue#200**.
		
7. Update the branch by:

	- Opening your browser and navigating to the appropriate folder on the **Code** tab of your GitHub fork. For example, if you changed a file that was in the **entries** sub-folder, make sure to select that sub-folder before proceeding.
	
	- Selecting **Add file** and then **Upload files**.
	
	- Dragging and dropping the changed file(s) from your local repository to the **Drag additional files here...** area.
	
	- Scrolling to the bottom of the page, adding a title to your change and any relevant descriptive information of the change. For example, a title could be **Fixes issue#189** and the description could be **This resolves a simple typographical issue in the breadcrumb** (assuming that issue #189 referred to resolving a single typographical issue in the breadcrumbs).
	
	- Selecting the **Commit directly** option.
	
8. Create a pull request to merge the content on the branch in your fork into the original repository by:

	- Opening a browser of your choice and navigating to the main page of your fork.
	
	- Selecting **Compare & Pull Request** button. 
	
	- Clicking **Compare across forks** and making sure that: 
		
		- The **Base repository** is the original repository.
		
		- The **base** branch is the default branch of the original repository.

		- The **Head Repository** is your fork.
		
		- The **compare** branch is the branch on your fork with the changed file(s). 
	
	- Reviewing and updating the title and description of the change, if necessary, and selecting **Create Pull Request**.
	
9. Because no one is supposed to merge their own pull request into the original repository, this portion of the workflow can be completed by:

	- Opening a browser, navigating to the appropriate original repository, selecting **pull request**, and selecting the appropriate pull request.
	
	- Selecting **Reviewers**.
	
	- Clicking on the search bar and selecting the name(s) of the reviewer(s) that you would like to review this pull request.
	
		- NOTE: Typically, someone assigned as a [**Maintainer**](maintenance) will be the person who will review and either approve or reject the pull request. 

<a href="#top">Return to top</a>
	
<h2 id="morecomline">Instructions for Contributing Changes (More Command Line)</h2>

1. Navigate to the appropriate original repository and review the issue you want to resolve.

	- NOTE: If you are not assigned to this issue, select **assign yourself** under **Assignees**.
	
	- NOTE: If an issue has not yet been created, contact a [**Maintenance**](maintenance) team member, who will create an issue for you.
	
	- NOTE: Review [**this video from Kate Flynn**](https://youtu.be/3fqsS2_ahXM) (from the time the video starts until 4:51) to learn more about how to review an issue.

2. Ensure your fork and local copy are in sync with the original repository by:

	- Opening your browser and navigating to the folder on your computer containing your local repository.
	
	- Typing and entering ```git fetch upstream``` into the command line tool (to fetch content from the original repository).
	
	- Typing and entering ```git checkout``` *and the name of your default branch* into the command line interface tool (to switch to the default branch). Typically, our default branch name for any DLF MAWG repository is **main**.
	
	- Typing and entering ```git merge upstream/``` *and the name of your upstream branch's default branch* into the command line interface tool. For example, this command could look like  ```git merge upstream/main```.
	
	- Typing and entering ```git push origin``` into the command line interface tool to push these changes to your fork, which will then update your fork. 
	
	    - NOTE: Typically, the nickname for your fork should be **origin** (and will be referred to as such in these instructions), but this could vary. Check your repository's nickname by typing ```git remote -v``` into the command line interface tool.

		- NOTE: If you encounter a message like **Your branch is up to date with 'origin/main,** then proceed to the next step. 
	
3. Fix the issue(s) in your local repository by:

	- Navigating to folder on your computer containing your local repository.
	
	- Opening the appropriate file(s) using the source code editor of your choice.
	
	- Making the appropriate change(s). 

4. Test that the issue has been resolved by:
	
	- Navigating to your command line interface tool, which should still be opened to your local repository.
	
	- Typing and entering ```bundle exec jekyll serve``` into your command line tool to start Jekyll locally on your computer.
	
	- Navigating to the provided **Server Address** (e.g. http://127.0.0.1:4000) and reviewing the change(s) that you made.

5. Once you're ready to push the changes to your fork, create a branch by:

	- Navigating to your command line interface tool, which should still be opened to your local repository.
	
	- Terminating the server by navigating to your command line tool, holding **Ctrl-C**, and typing and entering ```y``` until the command line interface window notes that the server has closed.
	
	- Typing ```git checkout -b``` *and a branch name* to simultaneously create a new local branch in your local repository and switch to that branch.
	
		- NOTE: Our branch naming convention is **issue#**, followed by a number that is the same as the issue number. For example, if the issue number is 200, the branch name would be **issue#200**.
		
6. Commit the changes to your branch by:

	- Navigating to your command line interface tool.

	- Typing and entering ```git add``` *and the file path(s) of the files that you changed*. You can also add all changed files by typing and entering ```git add .``` into a command line tool of your choice.
	
	- Typing and entering ```git commit -m``` *and a brief explanation of the change in quotation marks*. This will both commit your changes and add an explanatory message to your commit. For example, the text you could type and enter into your command line tool could be ```git commit -m "fixes issue#200```
	
	- Typing and entering ```git push --set-upstream``` *and fork nickname, followed by the branch number housing your change*. This will push the branch from your local repository to your fork. For example, the text you could type and enter into your command line tool could be ```git push --set-upstream origin main```
	
	- Finally, type and enter ```git checkout``` *and the name of your clone's default name* to return to the default branch in your local repository.
	
7. Create a pull request to merge the content on the branch in your fork into the original repository by:

	- Opening a browser of your choice and navigating to the main page of your fork.
	
	- Selecting **Compare & Pull Request** button. 
	
	- Clicking **Compare across forks** and making sure that: 
		
		- The **Base repository** is the original repository.
		
		- The **base** branch is the default branch of the original repository.

		- The **Head Repository** is your fork.
		
		- The **compare** branch is the branch on your fork with the changed file(s). 
	
	- Reviewing and updating the title and description of the change, if necessary, and selecting **Create Pull Request**.
	
8. Because no one is supposed to merge their own pull request into the original repository, this portion of the workflow can be completed by:

	- Opening a browser, navigating to the appropriate original repository, selecting **pull request**, and selecting the appropriate pull request.
	
	- Selecting **Reviewers**.
	
	- Clicking on the search bar and selecting the name(s) of the reviewer(s) that you would like to review this pull request.
	
		- NOTE: Typically, someone assigned as a [**Maintainer**](maintenance) will be the person who will review and either approve or reject the pull request. 
		
<a href="#top">Return to top</a>

<h2 id="revandappro">Reviewing and Approving Pull Requests</h2>

NOTE: A video detailing how to review a pull request from a forked repository is described in [**this YouTube video**](https://youtu.be/3fqsS2_ahXM).

When opening a pull request, you'll want to first scroll down and see if GitHub can merge the changes automatically. If this is the case, you'll see below the comments an alert like **This branch has no conflicts with the [default] branch.** There will also be a button that will let you merge the pull request automatically in this case. If there are branch conflicts, please reach out to a DLF MAWG group member listed in the [**Maintenance**](maintenance) page to resolve this issue.
	
However, it's general best practice to review the changes in a pull request before merging, even if there's nothing wrong. If you're reviewing changes from a fork, here's the steps you'll need to take to review changes:	

1. Review the **title** and **description** of the pull request.
	
2. Review the **Files Changed** tab to compare files and confirm that the change was substantially implemented. Consult the GitHub [**About comparing branches in pull requests page**](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-comparing-branches-in-pull-requests) if you require further instruction.
		
3. 	Confirm that the change will appear satisfactorily on the website by:

	- Opening a browser of your choice, navigating to the forked directory that you are reviewing, and copying the fork's URL. The URL can be found by clicking the **Code** button.
	
	- Navigating to the folder containing your local repository in your command line interface tool.
	
	- Typing and entering ```git remote add```, *followed by a nickname for the repository's fork that you will create and the URL that you just copied* into your command line tool. This will add the fork of the person who submitted the pull request to the list of repositories that you can access. An example would be ```git remote add sgfork https://github.com/GentrySteven/Sandbox.git```
	
	- Typing and entering ```git checkout```, *followed by the nickname for that fork that you just made as well as the branch housing the change that you're reviewing* into your command line tool. This will let you switch to the branch on the submitter's remote repository that you will need to review. 
		
	- Pulling the changes from the fork (**described in step 2 of this documentation**).
	
	- Running Jekyll (**described in step 4 of this documentation**) and reviewing the changes!
		
4. Once satisfied that this change is sufficient, approve the pull request by:

	- Clicking the **Merge Pull Request** drop-down arrow and ensuring that **Create a Merge Commit** is selected.

	- Selecting **Merge pull request**. 

<h2>Reverting Pull Requests</h2>

In the event that a pull request is erroneously merged into the default branch, you can immediately revert that pull request by:

1. Navigating to appropriate original repository in GitHub.

2. Clicking **Pull Requests**.

3. Clicking  **Closed**.

4. Clicking the appropriate closed pull request.

5. Clicking **revert** and approving the new pull request.

<a href="#top">Return to top</a>

<h2 id="otherwork">Other Workflows</h2> 

For other, maintenance-related workflows, consult our [**Maintenance**](maintenance) page.

<a href="#top">Return to top</a>

<h2>References</h2>

[**The official GitHub Documentation website**](https://docs.github.com/en).

Kate Flynn's original contribution instructions.