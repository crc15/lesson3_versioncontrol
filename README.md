# Project Name:  Lesson 3 Version Control


## Course Title:
Web Application Development

## Assignment Date:  
February 2, 2018

## Student Name:  
Caroline Cayll

## Project Description:
Summarizing 5 key concepts as well as learning how to use GitHub.

## Lessons Learned in the Assignment:
1. Version control: a system that records changes to a file or set of files over time so that you can recall specific versions later. There are various types of version control such as local, centralized, and distributed. Local version control systems consists of people copying files onto another directory. This method is common since it is very easy, but very accident prone as well. To deal with the issues, programmers developed local version control systems that had a simple database that kept all the changes to files under revision control. One of the more popular VCS tools is called RCS. It works by keeping patch sets, or the differences between files, in a special format on disk. Then it can re-create what any file looked like at any point in time by adding up all the patches.
2. Git has three main states that files can reside in. These include committed, modified, and staged. Commited is when the data is safely stored in your local database. Modified is when you have changed the file but have not committed it to your database yet. Lastly, staged is when you have marked a modified file in its current version to go into your next commit snapshot.This leads to the three main sections of a Git project: the Git directory, the working tree, and the staging area. The Git direcotry is where Git stores the metadata and object database for a project. This is the most important part of Git. In the working tree, files are pulled out of the compressed database in the Git directory and placed on disk for you to use or modify.The staging area is a file, usually in your Git directory, that stores information about what will go into your next commit. 
3. You can obtain a Git Repository one of two ways. The first way is taking a local directory that is currently not under version control, and turn it into a Git repository. The second way of obtaining a repository is to clone an existing Git repository from elsewhere. To initialize a repository in an existing directory, you first need to go to that project’s directory.This creates a new subdirectory named .git that contains all of your necessary repository files, a Git repository skeleton. At this point, nothing in your project is tracked yet. If you want to start version-controlling existing files, you should begin by tracking those files and do an initial commit. To clone an exisitng repository, you will need the command git clone. Git receives a full copy of nearly all data that the server has. Every version of every file for the history of the project is pulled down by default when you run git clone.
4. To remove a file from Git, you have to remove it from the tracked files (aka: remove it from your staging area) and then commit. The git rm command does that, and it also removes the file from your working directory so you don’t see it as an untracked file the next time.Sometimes, someone might want to keep the file on your hard drive but not have Git track it anymore.In other words, you can keep the file in your working tree but remove it from your staging area. This is good if you forgot to add something to your .gitignore file and accidentally staged it, like a large log file or a bunch of .a compiled files. To do this, use the --cached option. 
5. Git doesn’t explicitly track file movement. If you rename a file in Git, no metadata is stored in Git that tells it you renamed the file. However, Git is good at recognizing the movement after the fact. Git has a mv command and one that is equivelant to the mv command. Git figures out that it’s a rename implicitly, so it doesn’t matter if you rename a file the alternative method or with the mv command. The git mv is one command instead of three. It’s a convenience function. More importantly, you can use any tool you like to rename a file, and address the add/rm later, before you commit.

# lesson3_versioncontrol
