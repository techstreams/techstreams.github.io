---
layout: post
title: Google Drive as a Simple Git Host
tags: [google-drive, development]
---


**[Github](https://github.com/)**, **[Bitbucket](https://bitbucket.org/)**, **[GitLab](https://about.gitlab.com/)**, **[Google Cloud Source Repositories](https://cloud.google.com/source-repositories/docs/)** *and others* are fantastic ***[Git](https://en.wikipedia.org/wiki/Git_(software))*** hosting services.   But for personal projects and small team collaboration **[Google Drive](https://www.google.com/drive/)** can also provide a simple solution.  

<br>

---


## Overview

<br>

I've taken a several month writing hiatus during which I was able to develop some helpful [Google Apps Scripts](https://www.google.com/script/start/) which I hope to share in the future.  But in this and upcoming posts I want to ***focus on some personal workflows and tools*** I use to help me be more productive during script develop.

One such tool ... ***[Google Drive](https://www.google.com/drive/)*** ... can act as a ***simple Git host for backup and sharing*** of personal and collaborative small team script projects.  

Let's see how easy this is to set up.

<br>

---



## Setup Google Drive for Git Hosting

<br>



**STEP 1:** Download and Install [Google Drive](https://www.google.com/drive/download/) for your desktop and ensure [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) is installed on your system

<br> 

**STEP 2:** [Create a Git respository](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository) for your project

<br> 

**STEP 3:** From inside the project folder, create a **'bare' Git clone** of the repository on Google Drive using the following command

`git clone --bare . PATH_TO_GOOGLE_DRIVE_SYNC_FOLDER/ANY_SUBFOLDER_PATH/PROJECT_NAME.git`

*Example:*  `git clone --bare . ~/GoogleDrive/Git/addon.git`

<br> 

**STEP 4:** Configure a **Git remote** with the following command

`git remote add  REMOTE_NAME  PATH_TO_GOOGLE_DRIVE_SYNC_FOLDER/ANY_SUBFOLDER_PATH/PROJECT_NAME.git`

*Example:*  `git remote add gdrive ~/GoogleDrive/Git/addon.git`

<br> 

**STEP 5:** Push/Pull project changes to/from the remote ... *changes will sync with Google Drive*


*Example:* `git push gdrive master`

*or*  

*Example:* `git pull gdrive master`

<br>

---

## Share a Google Drive Hosted Git Project

<br>

*To share a Google Drive hosted Git project with collaborators:*

<br>

**STEP 1:** **[Share](https://support.google.com/drive/answer/2494822)** the Git repository folder with the collaborator(s) on Google Drive


<br>

*__Each collaborator__ should then:*

<br> 

**STEP 2:** Download and install [Google Drive](https://www.google.com/drive/download/) for desktop and ensure that [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) is installed on their system

<br> 

**STEP 3:** **[Sync](https://support.google.com/drive/answer/2375083?hl=en)** the shared Git project folder to their local Google Drive

<br> 

**STEP 4:** Execute the **Git clone** command for the shared project

`git clone PATH_TO_GOOGLE_DRIVE_SYNC_FOLDER/ANY_SUBFOLDER_PATH/PROJECT_NAME.git`


*Example:*  `git clone ~/GoogleDrive/Git/addon.git`

<br> 


**STEP 5:** Configure a **Git remote** for the shared project with the following command 

`git remote add REMOTE_NAME PATH_TO_GOOGLE_DRIVE_SYNC_FOLDER/ANY_SUBFOLDER_PATH/PROJECT_NAME.git`


*Example:* `git remote add gdrive ~/GoogleDrive/Git/addon.git`

<br> 

**STEP 6:** Push/Pull project changes to/from the remote ... *changes will sync with Google Drive*

*Example:* `git push gdrive master`

*or*

*Example:* `git pull gdrive master`

<br> 

<i class="fa fa-hand-o-right"></i> **BEST PRACTICE** - *If sharing the Git repository, collaborators should coordinate 'push' and 'pull' operations so as not to have sync conflicts which could leave the Git repository in an unstable state.*

---

<i class="fa fa-exclamation-circle"></i> *__[Dropbox](https://www.dropbox.com/)__ is another alternative for simple Git hosting.*


