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

<img src="./images/account_newrepo" style="width:200px;"/>

2) Fill out the fields to create a new repository.
3) Now we will clone this repository down to the local computer. Copy the URL displayed on your new repository page:

<img src="./images/account_httpsurl" style="width:200px;"/>

4) Open up the windows cmd.exe. You can find this by clicking the windows/start button and searching 'cmd'. It looks like this:

<img src="./images/git_cmd" style="width:200px;"/>

5) In the cmd window, you want to type 'git clone' and then paste the url from step 4.

The command should look like this, although the URL should be your own repository's URL:

`
 git clone https://github.com/jackg-ch/ch_labs.git
`

it will look like this:
<img src="./images/git_clone" style="width:200px;"/>



# Source Tree Github