---
sectionid: contributing-to-site
layout: page
title: Contributing Instructions
permalink: contributing-to-site
---

{::options parse_block_html="true" /}

<h2>Page Sections</h2>

<ul>
	<li><a href="#intro">Introduction</a></li>
	<li><a href="#workflowhigh">High Level Workflow</a></li>
	<li><a href="#mincomline">Instructions for Contributing Changes (Minimal Command Line)</a></li>
	<li><a href="#morecomline">Instructions for Contributing Changes (More Command Line)</a></li>
	<li><a href="#revandappro">Reviewing and Approving Changes</a></li>
	<li><a href="#otherwork">Other Workflows</a></li>
</ul>

<h2 id="intro">Introduction</h2>

[**Now that you have installed all necessary dependencies, as well as configured your repositories**](installation), you are ready to begin contributing changes!

To facilitate contributing to our website, we have provided two similar workflows:

- The first workflow primarily avoids the command line, and is envisioned as more appropriate for those who are entirely new to Git and GitHub.

- The second workflow employs more of the command line. *We recommend using the second workflow once you are comfortable with the command line, Git, GitHub, and the GitHub workflow.*

*Note*: Words in all capital letters indicate content that you need to supply.

<h2 id="workflowhigh">High Level Workflow</h2>

Regardless of which specific workflow you use, the general steps are the same:

1. Navigate to the appropriate original repository and review the issue(s) that you want to address.

2. Update your fork.

3. Update your local repository.

4. Use a text editor to make changes in your clone.

5. Test your clone to ensure that you have resolved the the issue(s).

6. Create a new branch to house your change.

7. Push the branch to your fork.

8. Create a pull request to merge the branch into the original repository.

9. Assign reviewers to review your pull request.

Once you have assigned one or more reviewer(s), they will:

1. Review the change.

2. Merge the pull request and delete the branch (if the change(s) is/are satisfactory).

3. Or, reach out to the change contributor to resolve the issue(s) before repeating the process outlined in step 2 (if the change(s) is/are not satisfactory).

<h2 id="mincomline">Instructions for Contributing Changes (Minimal Command Line)</h2> 

1. Navigate to the appropriate original repository and review the issue you want to resolve.

	- *Note*: If you are not assigned to this issue, select ```assign yourself``` under ```Assignees```.
	
	- *Note*: If an issue has not yet been created, contact a [**maintenance**](maintenance) team member, who will create an issue for you.
	
	- *Note*: Review this video from Kate Flynn (from the time the video starts until 4:51) to learn more about how to review an issue: [https://youtu.be/3fqsS2_ahXM?t](https://youtu.be/3fqsS2_ahXM).

2. Ensure that your fork is in sync with the original repository by:

	- Opening your command line interface and navigating to your fork.
	
	- Selecting the default branch.
	
	- Selecting ```Fetch Upstream```.
	
	- (Optionally) Select ```Compare``` and review.
	
	- Selecting ```Fetch and Merge```.
	
3. Ensure your local repository is in sync with your fork by:

	- Opening a command line terminal/prompt.
	
	- Navigating into the folder on your computer containing your local repository

	- Navigating into the folder containing the README file.

	- Typing the following into the terminal: ```git checkout DEFAULT BRANCH NAME``` (to make sure you are on the default branch).  The DLF MAWG's default branch name is typically called ```main```.

	- Typing and entering ```git pull origin DEFAULT BRANCH NAME```, which will pull and merge the material in your fork into your local repository.
		
	- *Note*: If you encounter a message like ```Your branch is up to date with 'origin/DEFAULT BRANCH NAME```, then proceed to the next step. 	
	
4. Fix the issue in your local repository by:

	- Navigating to the folder on your computer containing your local repository.
	
	- Opening the appropriate file(s) using the source code editor of your choice.
	
	- Making the appropriate change(s). 

5. Test that the issue has been resolved by:
	
	- Opening your command line prompt/terminal, and--if necessary--navigating to the directory containing the README file of your clone.
	
	- Running ```bundle exec jekyll serve``` to start Jekyll.
	
	- Navigating to the provided *Server Address* (e.g. http://127.0.0.1:4000) and reviewing the change(s) that you made.
	
	- Closing the command line prompt once you are satisfied with the change(s).

6. Once you're ready so implement the change, select or create the branch that will house that change by:
	
	- Opening a browser of your choice and navigating to your fork.
	
	- Selecting the branch drop-down menu, typing the name of your branch into the search bar, and choosing one of the following:
		
		- If you have already created a branch for this change, type that branch name into the search bar and select the branch.
		
		- If you need to create a new branch, type the name of the branch into the search bar and select the ```create branch``` option. Our branch naming convention is *issue#*, followed by a number for that issue number.
		
7. Update the branch by:

	- Opening your browser and navigating to the appropriate folder on the ```Code``` tab of your GitHub fork. For example, if you changed a file that was in the entries sub-folder, make sure you select that sub-folder before proceeding.
	
	- Selecting ```Add file``` and then ```Upload files```.
	
	- Dragging and dropping the changed file(s) from your local repository to the ```Drag additional files here...``` bar.
	
	- Scrolling to the bottom of the page, adding a title to your change and any relevant descriptive information of the change. For example, a title could be ```Fixes issue#0189``` and the description could be ```This resolves a simple typogaphical issue in the breadcrumb```.
	
	- Selecting the ```Commit directly``` option.
	
8. Create a pull request to merge the content on the branch in your fork into the original repository by:

	- Opening a browser of your choice and navigating to the main page of your fork.
	
	- Selecting the ```Compare & Pull Request``` button for the branch you just made.
	
	- Clicking ```Compare across forks``` and making sure that: 
		
		- The ```Base repository``` is the original repository.
		
		- The ```base``` branch is the default branch of the original repository.

		- The ```Head Repository``` is your fork.
		
		- The ```compare``` branch is the branch on your fork with the changed file(s). 
	
	- Reviewing and updating the title and description of the change, and selecting ```Create Pull Request```.
	
9. Because no one is supposed to merge their own pull request into the original repository, complete this workflow by:

	- Opening a browser, navigating to the appropriate original repository, and selecting the appropriate pull request.
	
	- Selecting ```Reviewers```.
	
	- Clicking on the search bar and selecting the name(s) of the reviewer(s) that you want to review this pull request.
	
		- *Note*: Typically, someone assigned to [**maintain**](maintenance) the DLF MAWG Website will be the person who will review and either approve or reject the pull request. 
	
<h2 id="morecomline">Instructions for Contributing Changes (More Command Line)</h2>

1. Navigate to the appropriate original repository and review the issue(s) that you want to resolve.

	- *Note*: If you are not assigned to this issue, select ```assign yourself``` under ```Assignees```.
	
	- *Note*: If an issue has not yet been created, contact a [**maintenance**](maintenance) team member, who will create an issue for you.
	
	- *Note*: Review this video from Kate Flynn (from the time the video starts until 4:51) to learn more about how to review an issue: [https://youtu.be/3fqsS2_ahXM?t](https://youtu.be/3fqsS2_ahXM).

2. Ensure your fork and local copy are in sync with the original repository by:

	- Opening your browser and navigating to the folder on your computer containing your project.
	
	- Typing and entering ```git fetch upstream``` into the command line terminal/prompt (to fetch content from the original repository).
	
	- Typing and entering ```git checkout main``` into the command line terminal/prompt (to switch to the default branch).
	
	- Typing and entering ```git merge BRANCHNAME``` into the command line terminal/prompt, where BRANCHNAME is the name of the branch (e.g. ```upstream/main```).
	
	- Typing and entering ```git push origin``` into the command line terminal/prompt to update your fork. Typically the nickname for your fork should be ```origin``` (and will be referred to as such in these instructions), but this could vary. Check your repository's nickname by typing ```git remote -v``` into the command line terminal/prompt.
		
	- *Note*: If you encounter a message like ```Your branch is up to date with 'origin/DEFAULT BRANCH NAME,``` then proceed to the next step. 
	
3. Fix the issue(s) in your local repository by:

	- Navigating to folder on your computer containing your local repository.
	
	- Opening the appropriate file(s) using the source code editor of your choice.
	
	- Making the appropriate change(s). 

4. Test that the issue has been resolved by:
	
	- Navigating to your command line prompt/terminal, which should still be opened to your local repository.
	
	- Running ```bundle exec jekyll serve``` to start Jekyll.
	
	- Navigating to the provided *Server Address* (e.g. http://127.0.0.1:4000) and reviewing the change(s) that you made.

5. Once you're ready to push the changes to your fork, create a branch by:

	- Opening your terminal.
	
	- Terminating the server by selecting Ctrl-C and entering ```y``` until the command line prompt/terminal notes the server has closed.
	
	- Typing ```git checkout -b BRANCHNAME``` to simultaneously create a new local branch in your local repository and switch to that branch. Our branch naming convention is *issue#*, followed by a number for that issue number.
		
6. Commit the changes to your branch by:

	- Navigating to your command line terminal/prompt.

	- Typing and entering ```git add``` and the file path(s) of the files that you changed. You can either add individual files or add all changed files. To do the latter, simply type  ```git add .```
	
	- Typing and entering ```git commit -m "fixes issue#NUMBER",``` where NUMBER is the issue number. This will both commit your changes and add an explanatory message to your commit.  
	
	- Typing and entering ```git push --set-upstream origin issue#NUMBER```, using the same branch name as in the previous step . This branch from your local repository should now be in your fork. 
	
	- Finally, type and enter ```git checkout DEFAULT BRANCHNAME``` to return to the default branch in your local repository.
	
7. Create a pull request to merge the content on the branch in your fork into the original repository by:

	- Opening a browser and navigating to the main page of your fork.
	
	- Selecting the ```Compare & Pull Request``` button for the branch you just made.
	
	- Clicking ```Compare across forks``` and making sure that: 
		
		- The ```Base repository``` is the original repository.
		
		- The ```base``` branch is the default branch of the original repository.

		- The ```Head Repository``` is your fork.
		
		- The ```compare``` branch is the branch on your fork with the changed file(s). 
	
	- Reviewing and updating the title and description of the change, and selecting ```Create Pull Request```.
	
8. Because no one is supposed to merge their own pull request into the original repository, complete this workflow by:

	- Opening a browser, navigating to the appropriate original repository, and selecting the appropriate pull request.
	
	- Selecting ```Reviewers```.
	
	- Clicking on the search bar and selecting the name(s) of the reviewer(s) that you want to review this pull request. Typically, someone assigned to [**maintain**](maintenance) the DLF MAWG Website will be the person who will review and either approve or reject the pull request. 

<h2 id="revandappro">Reviewing and Approving Changes</h2>

*Note*: A video detailing how to review a pull request from a forked repository is available on [**Youtube**](https://youtu.be/3fqsS2_ahXM).

When opening a pull request, you'll want to first scroll down and see if GitHub can merge the changes automatically. If this is the case, you'll see below the comments an alert that ```This branch has no conflicts with the master branch.``` There will also be a button that will let you merge the pull request automatically in this case. If there are branch conflicts, please reach out to a DLF MAWG group member listed in the [**Maintenance**](maintenance) page to resolve this issue.
	
However, it's general best practice to review the changes in a pull request before merging, even if there's nothing wrong. If you're reviewing changes from a fork, here's the steps you'll need to take to review changes:	

1. Review the title and description of the pull request.
	
2. Review the ```Files Changed``` tab to compare files and confirm that the change was substantially implemented. Consult the GitHub [**About comparing branches in pull requests**](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-comparing-branches-in-pull-requests) page if you require further instruction.
		
3. 	Confirm that the change will appear satisfactorily on the website by:

	- Opening a browser of your choice, navigating to the forked directory that you are reviewing, and copying the fork's URL. The URL can be found by clicking the ```Code``` button.
	
	- Navigating to the folder containing your local repository into your command line terminal/prompt.
	
	- Typing and entering ```git remote add NICKNAME FORKURL```, where NICKNAME is a nickname for the repository's that you will create and FORKURL is the URL that you just copied. This will add the submitter's forked repository and will let you switch to these branches. 
	
	- Typing and entering ```git checkout NICKNAME/BRANCHNAME``` to switch to the branch on the remote repository that you will need to review. 
		
	- Pulling the changes from the fork.
	
	- Runing Jekyll and review changes!
		
4. Once satisfied that this change is sufficient, approve the pull request by:

	- Clicking the ```Merge Pull Request``` drop-down arrow and ensuring that ```Create a Merge Commit``` is selected.

	- Selecting ```Merge pull request```. 
	
	- Deleting the merged branch.

<h2 id="otherwork">Other Workflows</h2> 

For other, maintenance-related workflows, consult our [**maintenance**](maintenance) page.

<h2>References</h2>

[The official GitHub Documentation website](https://docs.github.com/en).

Kate Flynn's original contribution instructions.