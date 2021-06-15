---
sectionid: installation-set-up
layout: page
title: Installation and Setting Up
permalink: installation
---

{::options parse_block_html="true" /}

# Introduction

Once you have a basic understanding of Git and GitHub, you will next need to:

1. Install several pieces of software.

2. Establish a GitHub profile and (optionally) become a contributor to the [DLFMetadataAssessment GitHub organization](https://github.com/DLFMetadataAssessment). 

3. Establish your necessary repositories.

We will begin with installation instructions, which have been provided for users with either Windows and macOS operating systems.

# Installation Overview

Regardless of the operating system that your computer uses, you will need to install the following:

- Git.

- Jekyll.

- Ruby (version 2.4 or higher), as well as relevant associated software (e.g. Bundler). 

- A source-code editor of your choosing, such as [Atom](https://atom.io/) or [Notepad++](https://notepad-plus-plus.org/).

Additionally, you will need to create a GitHub account if you have not already done so. 

# Installation Instructions (macOS)

**macOS users can select several different options to install necessary software. Very general installation instructions are provided below**:

1. Review the various [Git installation options on macOS](https://git-scm.com/download/mac) and select the Git option that works best for you. 

2. Review the instructions on the [Jekyll on macOS page](https://jekyllrb.com/docs/installation/macos/) and install the option that works best for you. **Note that if you're running macOS Big Sur 11.x, Ruby should already be installed on your computer.**

3. Test that Ruby has been installed by opening a terminal window and typing **ruby -v** into the terminal window. If the version number is returned, you have successfully installed Ruby.

4. [Install Jekyll and bundler](https://jekyllrb.com/docs/installation/macos/#install-jekyll). 

5. Install a source-code editor of your choice. [Atom](https://atom.io/) and [Visual Studio Code](https://code.visualstudio.com/) are two popular editors.

6. [Create a GitHub account](https://github.com/join) if you have not already done so. 

# Installation Instructions (Windows)

**Although not officially supported on Windows computers, Jekyll can still be run on those machines.**

1. [Download and install the appropriate Git for Windows](https://git-scm.com/download/win), depending on whether your computer is a 32-bit or 64-bit system.

2. Download and install a [a Ruby+Devkit from RubyInstaller](https://rubyinstaller.org/). During installation, do not change the default options and run ridk install when the option presents itself.

3. Test that Ruby has been installed by opening a comand prompt window and typing **ruby -v** into the command prompt window. If the version number is returned, you have successfully installed Ruby.

4. Open your command prompt and type **gem install jekyll bundler**. 

5. Test that Ruby has been installed by opening a comand prompt window and typing **jekyll -v** into the command line. If a version number is returned, Jekyll has been installed properly.

6. Install a source-code editor of your choice. [Atom](https://atom.io/), [Notepad++](https://notepad-plus-plus.org/), and [Visual Studio Code](https://code.visualstudio.com/) are two popular editors.

7. [Create a GitHub account](https://github.com/join) if you have not already done so. 

# Set Up Overview

Now that you have installed the necessary dependencies, it is time to set up the appropriate environments and become a contributor to the DLFMetadataAssessment GitHub organization!

# GitHub Repositories

When you're contributing changes to a repository like [DLFMetadataAssessment.github.io](https://github.com/DLFMetadataAssessment/DLFMetadataAssessment.github.io), you are actually interacting with several similar, but distinct, repositories:

- The original repository, which is accessible remotely via GitHub. **This is where the "official" or "final" version of the code and documentation lives.** [DLFMetadataAssessment/Sandbox](https://github.com/DLFMetadataAssessment/Sandbox) is an example of a **original repository.**

- The forked copy of the repository (or fork), which is also accessible remotely via GitHub. **Think of this repository as your personal staging area, from which you can incorporate changes into the official repository.** [kateefly/Sandbox](https://github.com/kateefly/Sandbox) is Kate Flynn's **fork** of the original repository.

- A cloned, or local, copy of the repository, which can be found on anywhere on your computer. **This is your personal workspace, where all the hard work happens!** A copy of the repository on Kate's Desktop is the **local copy** of the repository. 

The citation listed under our References section provides further explanation about the differences between original, forked, and cloned repositories. 

To establish a fork:

1. Navigate to the appropriate original repository.

2. Select the **fork** option and the appropriate GitHub profile.

To establish a local repository:

1. Create an empty folder at a place of your choosing to house your code.

2. Navigate to your fork.

3. Select the **Code ↓** option and select the copy button next to the URL.

4. Open a terminal of your choosing, such as Git Bash (which you just downloaded) or the Windows command prompt.

5. Using your terminal, navigate to the empty folder you just made.

6. Type **git clone**, paste the URL that you just copied into the terminal--so that the command now reads like git clone https://github.com/GentrySteven/Sandbox.git

7. **Enter** that URL into the prompt to finish making your local repository. 

Finally, [configure your repository](https://docs.github.com/en/github/collaborating-with-pull-requests/working-with-forks/configuring-a-remote-for-a-fork):

1. Open a terminal and navigate to the folder containing your local repository.

2. Navigate to the folder containing the **README file**.

3. Type into the terminal **git remote -v**. If you see any **upstream** repositories, proceed to the [Contributing to the Website](contributing-to-site) and begin making changes! Otherwise, continue to the next step.

4. Type **git remote add upstream ORIGINAL REPOSITORY GITHUB URL**. For example, to establish the Sandbox as an upstream repository, you would type git remote add upstream https://github.com/DLFMetadataAssessment/Sandbox. **Make sure you are 

5. **Enter** that command into the prompt.

6. Type **git remote -v** into the terminal. If you see any **upstream** repositories.

#Joining the DLFMetadataAssessment GitHub Organization (Optional)

Lastly, consider becoming a contributor to the [DLFMetadataAssessment GitHub organization](https://github.com/DLFMetadataAssessment). 

Joining an organization is not a requirement to contribute changes, but we recommend joining if you will be actively contributing to the organization!

To join the organization, please reach out the DLF MAWG group members listed in the [Maintenance](maintenance) page.

# Next Steps 

Proceed to the [Contributing to the Website](contributing-to-site) and begin making changes!

#References

[The difference between forking and cloning a repository](https://github.community/t/the-difference-between-forking-and-cloning-a-repository/10189).
