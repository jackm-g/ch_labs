# Getting Started with Github for Windows 10
- [Getting Started with Github for Windows 10](#getting-strted-with-github-for-windows-10)
  * [Install Git for Windows](#install-git-for-windows)
  * [Create a Github Account](#create-a-github-account)
  * [Create a Repository and Clone it](#create-a-repository-and-clone-it)
  * [Push Your Code up to Github](#push-your-code-up-to-github)
- [Source Tree Github](#source-tree-github)
## Install Git for Windows

**Steps**
1) Navigate to https://git-scm.com/downloads
2) Click the Windows link to begin the download.
3) Run the downloaded file and follow the install. Accept all default settings (just click next each time it asks)


## Create a Github Account

A github account allows you to create online repositories on https://www.github.com. We will make one so that we can put the code from the labs into these online repositories. This is helpful since we can save our work in a permanent way regardless of the computer we are using.

**Requirements**
- A valid email address you can access

**Steps**
1) Open a browser and navigate to https://github.com/join?source=header-home and follow the steps to create a github account.
2) Choose the Free account and complete the setup.

## Create a Repository and Clone it

**Steps**
1) Sign into your GitHub account and navigate to https://github.com/new

<img src="https://github.com/jackg-ch/ch_labs/blob/master/images/account_newrepo.PNG" width="500"/>

2) Fill out the fields to create a new repository.
3) Now we will clone this repository down to the local computer. Copy the URL displayed on your new repository page:

<img src="https://github.com/jackg-ch/ch_labs/blob/master/images/account_httpslink.PNG" width="700"/>

4) Open up the windows cmd.exe. You can find this by clicking the windows/start button and searching 'cmd'. It looks like this:

<img src="https://github.com/jackg-ch/ch_labs/blob/master/images/git_cmd.PNG" width="200"/>

5) In the cmd window, you want to type 'git clone' and then paste the url from step 4.

The command should look like this, although the URL should be your own repository's URL:

`
 git clone https://github.com/jackg-ch/ch_labs.git
`

it will look like this:

<img src="https://github.com/jackg-ch/ch_labs/blob/master/images/git_clone.PNG" width="400"/>

6) Now your repository's folder is on your computer. You should be able to view it by typing the `dir` command in the same directory you issued the `git clone` command. You can navigate to it with the `cd` command. In your cmd window type the following commands, replacing `<RepositoryFolderName>` with the name of the folder that matches your git repository name. If the folder is missing, you may be in the wrong directory or the repository did not clone down to your computer correctly. 

```
dir
cd <RepositoryFolderName>
```

When you issue the commands, the output of your cmd window should look like this:

```
D:\GitHub\test_dir>git clone https://github.com/jackg-ch/TestRepository.git
Cloning into 'TestRepository'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.

D:\GitHub\test_dir>dir
 Volume in drive D is nSSD
 Volume Serial Number is 3097-F7F9

 Directory of D:\GitHub\test_dir

10/17/2019  08:31 PM    <DIR>          .
10/17/2019  08:31 PM    <DIR>          ..
10/17/2019  08:31 PM    <DIR>          TestRepository
               0 File(s)              0 bytes
               3 Dir(s)  240,472,125,440 bytes free

D:\GitHub\test_dir>cd TestRepository

D:\GitHub\test_dir\TestRepository>
```


## Push Your Code up to Github

**Steps**
1) `cd` into the cloned repository folder if you haven't already. `cd <RepositoryFolderName>`
2) Let's make a simple text file to add to this repository. Open up your file explorer and navigate to the folder you just cloned down (your repository folder). 
Open it up and create a text file, write anything you want in it, and save it. To create a text file: `right click inside folder > new > Text Document`
3) Now that we have a new file, go back to the cmd.exe window you had open before. 
4) Type `git add .` and hit enter. Make sure you issue this command from inside your cloned github repository folder. This command tells your git repository
that you want to add all of the new files you've made to your repository.
5) Next, we will commit the files. This tells git that you are done adding files or making changes to them and wish to commit it to the repository's history. Type
`git commit -m "Any Message You Want"` (You can put any sentence you want inside the quotes, ideally one that describes the changes you made) and hit enter. 
6) However, you will probably get a message that says it did not work! We need to tell our computer's git tool who we are.
This can be done by issuing the command `git config user.email "your.email@gmail.com"`. This needs to be the same email you used for your github account. 
7) now re-type the `git commit -m "message"` command. once it completes, we are ready to push our changes up to the repository.
8) Type `git push` and hit enter. If this completes successfully you can now refresh your repository's webpage on github and see the files you've added. Congrats!

Note: You may get a window that prompty you for your Github username/password. Enter it and the command should complete successfully. It looks like this:

<img src="https://github.com/jackg-ch/ch_labs/blob/master/images/git_password.PNG" width="400"/>



The process of adding your code, making a commit, and pushing the code up should look like this in the cmd.exe window:
```
D:\GitHub\ch_labs>git add .

D:\GitHub\ch_labs>git commit -m "fix images"
[master a2f0cfb] fix images
 1 file changed, 4 insertions(+), 4 deletions(-)

D:\GitHub\ch_labs>git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 408 bytes | 204.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/jackg-ch/ch_labs.git
   c0c2dc3..a2f0cfb  master -> master

D:\GitHub\ch_labs>
```

If you wish to add other code to the repository: Open up your file explorer. Copy any code that you wish to add to the repository into the repository folder on your computer and issue the same `git add`, `git commit -m "<message here>"` and `git push` commands.

# Source Tree Github