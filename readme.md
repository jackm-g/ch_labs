# Github for Windows 10

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

<img src="https://github.com/jackg-ch/ch_labs/blob/master/images/account_newrepo.PNG" style="width:150px;"/>

2) Fill out the fields to create a new repository.
3) Now we will clone this repository down to the local computer. Copy the URL displayed on your new repository page:

<img src="https://github.com/jackg-ch/ch_labs/blob/master/images/account_httpslink.PNG" style="width:150px;"/>

4) Open up the windows cmd.exe. You can find this by clicking the windows/start button and searching 'cmd'. It looks like this:

<img src="https://github.com/jackg-ch/ch_labs/blob/master/images/git_cmd.PNG" style="width:100px;"/>

5) In the cmd window, you want to type 'git clone' and then paste the url from step 4.

The command should look like this, although the URL should be your own repository's URL:

`
 git clone https://github.com/jackg-ch/ch_labs.git
`

it will look like this:
<img src="https://github.com/jackg-ch/ch_labs/blob/master/images/git_clone.PNG" style="width:150px;"/>



## Push Your Code up to Github



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



# Source Tree Github