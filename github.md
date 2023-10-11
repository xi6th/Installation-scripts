# Step 1: Gh Installation

```
sudo apt install gh

```

Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following NEW packages will be installed:
  gh
0 upgraded, 1 newly installed, 0 to remove and 150 not upgraded.
Need to get 6,242 kB of archives.
After this operation, 33.7 MB of additional disk space will be used.
Get:1 http://ng.archive.ubuntu.com/ubuntu jammy/universe amd64 gh amd64 2.4.0+dfsg1-2 [6,242 kB]
Fetched 6,242 kB in 4s (1,426 kB/s)
Selecting previously unselected package gh.
(Reading database ... 212059 files and directories currently installed.)
Preparing to unpack .../gh_2.4.0+dfsg1-2_amd64.deb ...
Unpacking gh (2.4.0+dfsg1-2) ...
Setting up gh (2.4.0+dfsg1-2) ...
Processing triggers for man-db (2.10.2-1) ...

# Step 2: Authentication

```
gh auth login
```

? What account do you want to log into? GitHub.com
? What is your preferred protocol for Git operations? SSH
? Upload your SSH public key to your GitHub account? /home/xi6th/.ssh/id_rsa_personal.pub
? How would you like to authenticate GitHub CLI? Login with a web browser

! First copy your one-time code: 5D2D-D963

- Press Enter to open github.com in your browser...
  Opening in existing browser session.
  ✓ Authentication complete. Press Enter to continue...
- gh config set -h github.com git_protocol ssh
  ✓ Configured git protocol
  HTTP 422: Validation Failed (https://api.github.com/user/keys)
  key is already in use

# Step 3: Create Repo

```
gh repo create

```

? What would you like to do? Create a new repository on GitHub from scratch


? Repository name Installation scripts
? Description commands to install software and troubleshoot issues
? Visibility Public
? Would you like to add a .gitignore? No
? Would you like to add a license? Yes
? Choose a license Mozilla Public License 2.0
? This will create "Installation-scripts" as a public repository on GitHub. Continue? Yes
✓ Created repository xi6th/Installation-scripts on GitHub
? Clone the new repository locally? Yes
Cloning into 'Installation-scripts'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), 5.78 KiB | 5.78 MiB/s, done.

gh
