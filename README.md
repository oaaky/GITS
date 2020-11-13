
# GITS 
### GIT Simplified

![GitHub](https://img.shields.io/github/license/harshitpatel96/GITS)
[![Build Status](https://travis-ci.com/harshitpatel96/GITS.svg?branch=master)](https://travis-ci.com/harshitpatel96/GITS)
[![codecov](https://codecov.io/gh/harshitpatel96/GITS/branch/master/graph/badge.svg?token=G6RG52G2YO)](https://codecov.io/gh/harshitpatel96/GITS/)
![YouTube Video Views](https://img.shields.io/youtube/views/6Y8_RQecnZ8?style=social)

[![DOI](https://zenodo.org/badge/295480790.svg)](https://zenodo.org/badge/latestdoi/295480790)

![GitHub issues](https://img.shields.io/github/issues/harshitpatel96/GITS)
![GitHub closed issues](https://img.shields.io/github/issues-closed/harshitpatel96/GITS)

![Lines of code](https://img.shields.io/tokei/lines/github/harshitpatel96/GITS)

[![](https://img.youtube.com/vi/6Y8_RQecnZ8/hqdefault.jpg)](https://youtu.be/6Y8_RQecnZ8 "GITS demo")

# About GITS
GITS streamlines most frequently performed workflows using fewer commands which is so much easier and better than usual.
Git-Simplified AKA GITS can be thought of wrapper around major Git functionalities.

# Installation for Linux
1. Clone GITS Repo
2. From the root directory run the following command
    ```
    pip install -r requirements.txt
    ```
3. Go to configurations directory and run the following command

    If you are working on Linux system with a bash terminal or a Windows system using Windows subsystem for linux:
    ```
    bash project_init.sh
    ```
    If you are working on Linux system with a fish terminal:
    ```
    fish project_init.fish
    ```
   
# Installation for Windows
1. Clone GITS Repo
2. From the root directory run the following command
    ```
    pip install -r requirements.txt
    ```
3. Currently, this project cannot be run on Windows. You need to make use of WSL to work on this project in Windows 
although this fix would only work for systems running Windows 10. If you are using another version of Windows, using a 
virtual machine might be preferred.

    Please refer this link to enable WSL : https://docs.microsoft.com/en-us/windows/wsl/install-win10

# How to Contribute?
Please take a look at our CONTRIBUTING.md where we provide instructions on contributing to the repo and help us in enhancing the current video conferencing platforms.

# Documentation
## Functionalities Implemented
1. [gits profile](https://github.com/harshitpatel96/GITS/blob/master/docs/profile.md)
1. [gits rebase](https://github.com/harshitpatel96/GITS/blob/master/docs/rebase.md)
1. [gits reset](https://github.com/harshitpatel96/GITS/blob/master/docs/reset.md)
1. [gits upstream](https://github.com/harshitpatel96/GITS/blob/master/docs/upstream.md)
1. [gits super reset](https://github.com/harshitpatel96/GITS/blob/master/docs/super_reset.md)
1. [gits commit](https://github.com/harshitpatel96/GITS/blob/master/docs/commit.md)
1. [gits create_branch](https://github.com/harshitpatel96/GITS/blob/master/docs/create_branch.md)
1. [gits logging](https://github.com/harshitpatel96/GITS/blob/master/docs/logging.md)
1. [gits undo](https://github.com/harshitpatel96/GITS/blob/master/docs/undo.md)
1. [gits untrack](https://github.com/harshitpatel96/GITS/blob/master/docs/untrack.md)
1. [gits track](https://github.com/harshitpatel96/GITS/blob/master/docs/track.md)
1. [gits delete](https://github.com/harshitpatel96/GITS/blob/master/docs/delete.md)
1. [gits sync](https://github.com/harshitpatel96/GITS/blob/master/docs/sync.md)
1. [gits switch](https://github.com/harshitpatel96/GITS/blob/master/docs/switch.md)
1. [gits status](https://github.com/harshitpatel96/GITS/blob/master/docs/status.md)
1. [gits branch](https://github.com/harshitpatel96/GITS/blob/master/docs/branch.md)
1. [gits diff](https://github.com/harshitpatel96/GITS/blob/master/docs/diff.md)
1. [gits init](https://github.com/harshitpatel96/GITS/blob/master/docs/init.md)
1. [gits merge](https://github.com/harshitpatel96/GITS/blob/master/docs/merge.md)
1. [gits push](https://github.com/harshitpatel96/GITS/blob/master/docs/push.md)
1. [gits pull](https://github.com/harshitpatel96/GITS/blob/master/docs/pull.md)


## Pydoc implementation
We have tried to write as much documentation as possible. You can use pydoc to go through the documentation. 
For example if you want to go through all the documentation for all files in code/ directory, do the following: 

`cd code`<br>
`python3 -m pydoc -b `

This will open up a browser and you can see all the files. You can click on a particular file to access the 
documentation associated with that file.

This repository is made for CSC 510 Software Engineering Course at NC State University.


## Experimentation setup for phase 3

This project aims to ease the developers efforts while interacting with version control system Git. 
Here are few motivation points behind coming up with this idea:
- Few git command names are very misleading from the end user's perspective. Consider this, ```git checkout``` command is used for both switching the branches and removing changes present inside working directory.
- Based on the development practice used by various teams, there are some tasks which requires the execution of more than one command to complete the task. This process can be easily automated such that developer only need to execute a single command to get their work done.
- There are almost always the cases that because of not much efficient syncing techniques, code pushed to the remote repository results in conflict while merging. It is always best practice to solve any such merge conflicts on the local repo rather than the remote one.

To solve the issues described above, we came up with the project **gits** that stands for **git-Simplified**.
So, this experiment aims to compare various aspects to traditional git and our proposed gits.

### Participation

Basic idea here is to let the participants finish the tasks present in the tasks list mentioned below, and observe whether gits made this process easier or not. 
This is higher level idea for this study.
There are two ways to choose who will use git and who will use gits.
1. If you have significant number of participants, you can divide them up into two groups. Participants from one group will use Gits to complete the set of tasks while participants from second group will use traditional Git to finish their tasks. 
to achieve some great results, participants with lesser git knowledge should be assigned to later group who will be using git to finish their task. That would lessen the bias in observations since people would be already familiar with git rather than gits.
2. If number of participants are limited and have enough time, you can let each participants finish the set of tasks twice. Once using traditional git and then using gits.
However, to remove any unwanted bias here as well, divide the participants in two groups. first group should use the git first and then gits. Second group should finish the tasks using gits first and then using git.

Ask each participants to setup the gits inside their local machine before starting the study using steps shown above.

### Tasks list
In the first phase of experiment, please use only GITS command only to perform the git related tasks.
Similary in the second phase of experiment, please use only regular GIT commands.

You are given a repository by the person hosting the session. Work on that repository.
1. Clone the given repo
2. Add Your username and Email to the git configuration
3. Create Branch “branch1”.
4. Switch to main branch
5. Create Branch “branch2”
6. Switch to branch “branch1”
#### Branch1 tasks
7. Create file “test1.txt” and add `"hello test1"` in file
8. Stage the “test1.txt” file
9. Create file “test2.txt” and add `"hello test2"` in file
10. Stage the “test2.txt” file
11. Commit the changes and add `"my first commit"` commit message to it
12. Change the content of “test2.txt”  file from "hello test2" to `"hello test2 new"`.
13. Stage the file “test2.txt”.
14. Unstage the file “test2.txt”.
15. Remove the uncommitted changes made to the file “test2.txt”.
16. Switch to main branch.
17. Merge the branch branch1 to main branch.
#### Branch2 tasks
18. Switch to branch “branch2”.
19. Make “branch2” upto date with local main branch
20a. By this time, your remote main branch is updated by the host of your session. If not, confirm with the host.
20b. Make “branch2” upto date with remote main branch.
#### Main branch tasks
21. Switch to main branch
22. Delete the latest 1 commit from local as well as remote “main” branch
23. Suppose you have messed up the repo. You want to delete the local repo and re-clone it. Do it.

### Quantitative measures
Here are some measures that can help compare the results between traditional git and gits.
1. Time taken to finish a particular task.
2. Number of commands executed to complete each task.
3. Number of time participants referred to the documentation or any other resources.

### Qualitative measures
Along with quantitative measures described above, few qualitative measures can help to assess the performance better.
1. Familiarity with traditional git
2. hardness of the task
