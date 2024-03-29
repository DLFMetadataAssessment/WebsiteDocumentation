---
sectionid: installation-set-up
layout: page
title: Installation and Setting Up
permalink: installation
---

{::options parse_block_html="true" /}

<h2 id="top">Page Sections</h2>

<ul>
	<li><a href="#installover">Installation Overview</a></li>
	<li><a href="#git">Installing Git</a></li>
	<li><a href="#rubyjekyll">Installing Ruby, Jekyll, and Related Software</a></li>
	<li><a href="#setupover">Setting Up: Overview</a></li>
	<li><a href="#githubaccount">GitHub Account Creation and Configuring Git</a></li>
	<li><a href="#githubrepos">GitHub Repositories</a></li>
	<li><a href="#joindlf">Joining the DLFMetadataAssessment GitHub Organization (Optional)</a></li>
	<li><a href="#nextsteps">Next Steps</a></li>
</ul>

<h2>Introduction</h2>

[**Once you have a basic understanding of Git and GitHub**](before-you-begin), you will need to:

1. Install several pieces of software.

2. Establish a GitHub profile and (optionally) become a contributor to the [**DLFMetadataAssessment GitHub organization**](https://github.com/DLFMetadataAssessment). 

3. Establish your GitHub repositories.

If you have already installed the appropriate software and set up your environments, please navigate to [**the Contributing Changes**](contributing-to-site) page.

<h2 id="installover">Installation Overview</h2>

Regardless of your computer's operating system, you will need to install the following:

- Git.

- Ruby, as well as relevant associated software (e.g. Bundler). 

- Jekyll.

- A source-code editor of your choosing.

You will also need to create a GitHub account if you do not already have one. 

<a href="#top">Return to top</a>

<h2 id="git">Installing Git</h2>

Before you try to install Git, open a command line prompt (Windows) or terminal (macOS), and type and enter ```git --version```. If a Git version number is returned, Git is already installed on your computer (and you can skip this step). However, if a Git version is not returned, you will need to install Git.

Follow these instructions to install Git:

1. Navigate to the main [**Git**](https://git-scm.com/) website.

2. Click on **Downloads**.

3. Select the appropriate installation method, based on your computer's operating system (e.g. **Windows, macOS, Linux**).

4. Open the downloaded file and follow the instructions to install Git.

5. Test to make sure Git was installed by opening a command prompt (Windows) or terminal (macOS), and typing and entering ```git --version```. If a Git version number is returned, Git is installed on your computer. 

<a href="#top">Return to top</a>

<h2 id="rubyjekyll">Installing Ruby, Jekyll, and Related Software</h2>

Before you try to install to install Ruby, open a command line prompt (Windows) or terminal (macOS), and type and enter ```ruby -v```. Next, type and enter ```jekyll -v``` into that same command line window. 

If you get a Ruby and Jekyll version number, then both are already installed on your computer (and you can skip this step). However, if you do not get a Ruby version number, followed by a Jekyll version number, you will need to follow the [**Jekyll installation guide**](https://jekyllrb.com/docs/installation/) for your computer's particular operating system.

Finally, you will need to install a source-code editor of your choosing. Some popular editors include:

- [**Notepad++**](https://notepad-plus-plus.org/).

- [**Visual Studio Code**](https://code.visualstudio.com/).

<a href="#top">Return to top</a>

<h2 id="setupover">Setting Up: Overview</h2>

Now that you have installed the necessary software, it is time to create your GitHub account and set up the appropriate environments!

<a href="#top">Return to top</a>

<h2 id="githubaccount">GitHub Account Creation and Configuring Git</h2>

If you have not already done so, [**create a GitHub account**](https://github.com/join) and make sure that you have [**configured your username and email**](https://docs.github.com/en/get-started/quickstart/set-up-git#setting-up-git). 

<a href="#top">Return to top</a>

<h2 id="githubrepos">GitHub Repositories</h2>

Next, you will need to set up your various GitHub repositories.

When you're contributing changes to a repository like [**DLFMetadataAssessment.github.io**](https://github.com/DLFMetadataAssessment/DLFMetadataAssessment.github.io), you are actually interacting with several similar, but distinct, repositories:

- The original, or upstream, repository that is accessible remotely via GitHub. This is where the official version of the code and documentation lives. [**DLFMetadataAssessment/Sandbox**](https://github.com/DLFMetadataAssessment/Sandbox) is an example of an original repository.

- The forked copy of the original repository (or fork), which is accessible remotely via GitHub. Think of this repository as your personal staging area, from which you can incorporate your changes into the original repository. [**kateefly/Sandbox**](https://github.com/kateefly/Sandbox) is Kate Flynn's fork of the original Sandbox repository listed above.

- A cloned, or local, copy of the repository, which can be found anywhere on your computer. This is your personal workspace, where all the hard work happens! A copy of either the original or forked repository on Kate's computer is the local copy. 

Because the original repository already exists, you will only need to establish your fork and local copy. 

To establish a fork:

1. Navigate to the appropriate original repository.

2. Select the **fork** option and your GitHub profile.

To establish a local repository:

1. Create an empty folder, at a place of your choosing on your computer. This will house your local copy.

2. Open a browser and navigate to your fork.

3. Select the **↓ Code** option and select the **copy** button.

4. Open a command line tool of your choosing, such as Git Bash (which you just downloaded), macOS terminal, or the Windows command prompt.

5. Using your command line tool, navigate to the empty folder you just made. For example, if you are using a Windows or macOS computer, you would type ```cd``` and the *file path containing your local repository*.  

6. Type ```git clone``` and *the URL that you just copied into the command line tool*. Hit the enter/return key to download the code to the folder. 

7. Check your local repository folder to ensure that the code has been downloaded.

Finally, [**make sure to configure your repository**](https://docs.github.com/en/github/collaborating-with-pull-requests/working-with-forks/configuring-a-remote-for-a-fork):

1. Open a command line tool of your choice and, using the instructions above as a guide, navigate to the folder containing your local repository.

2. Navigate down to the folder containing the local copy's README file.

3. Type and enter ```git remote -v``` into the command line tool. 

If you see one or more upstream repository URLs in your command line interface window, proceed to the [**Contributing Changes**](contributing-to-site) page and begin making changes! However, if you only see origin repositories (e.g. your fork):

1. Type and enter ```git remote add upstream``` *and the original repository url*. For example, to establish the DLF MAWG Sandbox as an upstream repository, you would type ```git remote add upstream https://github.com/DLFMetadataAssessment/Sandbox```. 

2. Now, type ```git remote -v``` into command line interface window. If you see both upstream and origin repositories, you can proceed to the [**Contributing Changes**](contributing-to-site) page and begin making changes. 

If you continue to have issues, reach out to a [**DLF MAWG maintainer**](maintenance).

<a href="#top">Return to top</a>

<h2 id="joindlf">Joining the DLFMetadataAssessment GitHub Organization (Optional)</h2>

Optionally, consider becoming a contributor to the [**DLFMetadataAssessment GitHub organization**](https://github.com/DLFMetadataAssessment). 

Joining an organization is not a requirement to contribute changes, but we recommend doing so if you will be actively contributing to the DLF MAWG website!

To join the organization, please reach out to one of the DLF MAWG group members listed in the [**Maintenance**](maintenance) page.

<a href="#top">Return to top</a>

<h2 id="nextsteps">Next Steps</h2>

Once you've set up your environments, you are ready to begin [**contributing to a DLF MAWG repository**](contributing-to-site).

<a href="#top">Return to top</a>
