# UofS-KoLab (GitHub)
This organization is a comprehensive collection of projects undertaken by the current and graduated students of UofS KoLab under the supervision of Dr. Seokbum Ko.

Owner: Dr. Seokbum Ko (seokbum.ko@usask.ca)  
Maintainer: M. Hamis Haider (hamis.haider@usask.ca)  

## Table of contents
- [UofS-KoLab (GitHub)](#uofs-kolab-github)
  - [Table of contents](#table-of-contents)
  - [Manners \& Guidelines](#manners--guidelines)
  - [Deploying a repo on A40-Server](#deploying-a-repo-on-a40-server)
    - [1. Generating a deploy key](#1-generating-a-deploy-key)
    - [2. Adding the deploy key to your repo](#2-adding-the-deploy-key-to-your-repo)
    - [3. Cloning your repo](#3-cloning-your-repo)


## Manners & Guidelines
1. Cleanup after youself. Do regular cleanup of unnecessary materials and repositories in the organization.
2. Always open pull requests to merge into the default (main) branch of repos.
3. Always open issues to keep track of the project contributions and progress.
4. Use the github projects for task management sparingly.
5. Write device and os agnostic code wherever possible.
6. Write meangingful commit messages.
7. Always commit small changes and push. Big commits are harder to debug.
8. Ensure that project is in a "running" state locally before pushing to `dev` or `main` branch.

## Deploying a repo on A40-Server
> [!NOTE]
> It is advised that you use read-only deploy keys on the a40 server.


First, decide on a one word nickname for your repo. For example: `repo1`. It is helpful for your sake, if the nickname is meaningful and unique.  

Next we will assume your own nickname on the server. For example: `user1`.  

With these two nicknames in mind, follow the rest of the steps. These nicknames will come up often in the rest of the instructions.

### 1. Generating a deploy key
Once you've accessed the A40-server using Anydesk, open a terminal window and run the following command:
```bash
ssh-keygen -t ed25519 -C "user1-repo1"
```
Eventually you'll see the following prompt:
```
> Enter a file in which to save the key (/home/YOU/.ssh/id_ed25519): [Type the path mentioned below]
```
Enter the following path: `/home/uofsko-lab/.ssh/id_user1_repo1`, and then press **ENTER** key.  

Next you'll be asked for a passphrase. 
```
> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]
```
You can choose to leave it blank, but we encourage you to secure your key with a passphrase. 

### 2. Adding the deploy key to your repo

### 3. Cloning your repo
