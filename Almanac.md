# Git

`git clone "repository link"`

`git add .`

`git commit -m "commit message"`

`git push`

`git pull`

`git branch` : check branches present

`git checkout -b "branch_name"` : creates a branch with branch_name

`git commit -am "commit message"` : both adds and commits only modified files

`git merge master` : merges branch with master

`ssh-keygen -t ed25519 -C "email ID"`

copy contents of `/home/.ssh/id_ed25519.pub` to Github SSH keys

`git config --global user.name "Name"`

`git config --global user.email "Email"`


# Jupyter & SSH

In remote system:

`jupyter notebook --no-browser --port 8080`

In local system:

`ssh -N -f -L localhost:8080:localhost:8080 username@ip_addr` : Now go to browser and type URL http://localhost:8080

`lsof -ti:8080 | xargs kill -9` : clears any process running on port 8080


# Screen

`$ screen` : launch screen

`^A = Ctrl+a`

`^A ?` : all help

`^A c` : New screen

`^A A` : Rename screen

`^A num` : Switch using screen num

`^A d` : Detach from screen session

`^A "` : list all the screens

`screen -ls` : list all the running screen sessions from bash

`screen -r session_number` : run the screen of the particular session_num

# Linux

`sudo dpkg -i example.deb` : install using .deb files
