---
sectionid: installation-set-up
layout: page
title: Installation and Setting Up
permalink: installation
---

{::options parse_block_html="true" /}

<h2>Page Sections</h2>

<ul>
	<li><a href="#intro">Introduction</a></li>
	<li><a href="#installover">Installation Overview</a></li>
	<li><a href="#git">Installing Git</a></li>
	<li><a href="#rubyjekyll">Installing Ruby, Jekyll, and Related Software</a></li>
	<li><a href="#setupover">Setting Up: Overview</a></li>
	<li><a href="#githubaccount">GitHub Account Creation and Configuring Git</a></li>
	<li><a href="#githubrepos">GitHub Repositories</a></li>
	<li><a href="#joindlf">Joining the DLFMetadataAssessment GitHub Organization (Optional)</a></li>
	<li><a href="#nextsteps">Next Steps</a></li>
</ul>

<h2 id="intro">Introduction</h2>

[**Once you have a basic understanding of Git and GitHub**](before-you-begin), you will need to:

1. Install several pieces of software.

2. Establish a GitHub profile and (optionally) become a contributor to the [**DLFMetadataAssessment GitHub organization**](https://github.com/DLFMetadataAssessment). 

3. Establish your GitHub repositories.

If you have already installed the appropriate software and set up your environments, please navigate to [**the Contribution instructions**](contributing-to-site) page.

*Note*: Words in all capital letters indicate content that you need to supply.

<h2 id="installover">Installation Overview</h2>

Regardless of your computer's operating system, you will need to install the following:

- Git.

- Ruby, as well as relevant associated software (e.g. Bundler). 

- Jekyll.

- A source-code editor of your choosing.

You will also need to create a GitHub account if you do not already have one. 

<h2 id="git">Installing Git</h2>

Before you try to install to install Git, open a command prompt (Windows) or terminal (macOS), type ```git --version``` and hit *enter*. If a Git version number is returned, Git is already installed on your computer (and you can skip this step). However, if a Git version is not returned, you will need to install Git.

Follow these instructions to install Git:

1. Navigate to the main [Git](https://git-scm.com/) website.

2. Click on Downloads.

3. Select the appropriate installation method, based on your computer's operating system (e.g. Windows, macOS, Linux).

4. Open the downloaded file and follow the instructions to install Git.

5. Test to make sure Git was installed by opening a command prompt (Windows) or terminal (macOS), typing ```git --version``` and hitting enter. If a Git version number is returned, Git is installed on your computer. 

<h2 id="rubyjekyll">Installing Ruby, Jekyll, and Related Software</h2>

Before you try to install to install Ruby, open a command prompt (Windows) or terminal (macOS), type ```ruby -v``` and hit *enter*.  Next,  type ```jekyll -v``` and hit *enter*. 

If you get a Ruby and Jekyll version number, then both are already installed on your computer (and you can skip this step). However, if you do not get a Ruby version number, followed by a Jekyll version number, you will need to follow the [**Jekyll installation guide**](https://jekyllrb.com/docs/installation/) for your computer's particular operating system.

Finally, you will need to install a source-code editor of your choosing. Some popular editors include:

- [**Atom**](https://atom.io/).

- [**Notepad++**](https://notepad-plus-plus.org/).

- [**Visual Studio Code**](https://code.visualstudio.com/).

<h2 id="setupover">Setting Up: Overview</h2>

Now that you have installed the necessary software, it is time to create your GitHub account and set up the appropriate environments!

<h2 id="githubaccount">GitHub Account Creation and Configuring Git</h2>

If you have not already done so, [**create a GitHub account**](https://github.com/join) and make sure that you have [**configured your username and email**](https://docs.github.com/en/get-started/quickstart/set-up-git#setting-up-git). 

<h2 id="githubrepos">GitHub Repositories</h2>

Next, you will need to set up your various GitHub repositories.

When you're contributing changes to a repository like [**DLFMetadataAssessment.github.io**](https://github.com/DLFMetadataAssessment/DLFMetadataAssessment.github.io), you are actually interacting with several similar, but distinct, repositories:

- The original, or upstream repository that is accessible remotely via GitHub. This is where the *official* version of the code and documentation lives. [**DLFMetadataAssessment/Sandbox**](https://github.com/DLFMetadataAssessment/Sandbox) is an example of a original repository.

- The forked copy of the original repository (or fork), which is hosted on, and accessible remotely via, GitHub. Think of this repository as your personal staging area, from which you can incorporate your changes into the original repository. [**kateefly/Sandbox**](https://github.com/kateefly/Sandbox) is Kate Flynn's fork of the original Sandbox repository listed above.

- A cloned, or local, copy of the repository, which can be found anywhere on your computer. This is your personal workspace, where all the hard work happens! A copy of either the original or forked repository on Kate's computer is the local copy. 

Because the original repository already exists, you will only need to establish your fork and local copy. 

To establish a fork:

1. Navigate to the appropriate original repository.

2. Select the fork option and your GitHub profile.

To establish a local repository:

1. Create an empty folder, at a place of your choosing on your computer. This will house your clone.

2. Open a browser and navigate to your fork.

3. Select the ```↓ Code``` option and select the copy button.

4. Open a terminal of your choosing, such as Git Bash (which you just downloaded), macOS terminal, or the Windows command prompt.

5. Using your terminal, navigate to the empty folder you just made. For example, if you are using a Windows or macOS computer, you would type ```cd PATH TO LOCAL REPOSITORY FOLDER``` .

6. Type ```git clone```, paste the URL that you just copied into the terminal/prompt, and hit *enter* button. This will download the code to the folder. 

7. Check your local repository folder to ensure that the code has been downloaded.

Finally, [**configure your repository**](https://docs.github.com/en/github/collaborating-with-pull-requests/working-with-forks/configuring-a-remote-for-a-fork):

1. Open a terminal/prompt and navigate to the folder containing your local repository.

2. Navigate down to the folder containing the README file.

3. Type into the terminal ```git remote -v```. 

If you see one or more upstream repository URLs in the command line terminal/prompt window, proceed to the [**Contributing to the Website**](contributing-to-site) page and begin making changes! However, if you only see origin repositories (e.g. your fork):

1. Type ```git remote add upstream ORIGINAL REPOSITORY URL```. For example, to establish the DLF MAWG Sandbox as an upstream repository, you would type ```git remote add upstream https://github.com/DLFMetadataAssessment/Sandbox```. 

2. *Enter* that command into the prompt.

3. Now, type ```git remote -v``` into the terminal. If you see both upstream and origin repositories, you can proceed to the [**Contributing to the Website**](contributing-to-site) page and begin making changes. If you continue to have issues, reach out to a [**maintenance**](maintenance) volunteer.

<h2 id="joindlf">Joining the DLFMetadataAssessment GitHub Organization (Optional)</h2>

Optionally, consider becoming a contributor to the [**DLFMetadataAssessment GitHub organization**](https://github.com/DLFMetadataAssessment). 

Joining an organization is not a requirement to contribute changes, but we recommend doing so if you will be actively contributing to the DLF MAWG website!

To join the organization, please reach out the DLF MAWG group members listed in the [**Maintenance**](maintenance) page.

<h2>References</h2>

[**The difference between forking and cloning a repository**](https://github.community/t/the-difference-between-forking-and-cloning-a-repository/10189).
