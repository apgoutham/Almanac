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

Convert ipynb to py

`jupyter nbconvert --to script file.ipynb file.py`



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

`rename 's/[M]//g' *.jpg` : rename all jpg filenames with replacing `M` with nothing


# Python
In case of errors like `matplotlib: cannot connect to X server localhost:10.0` : In terminal, type: `export DISPLAY=localhost:11.0`

# Vim
To print: 001_06 002_06 // 001_06 002_07 // etc..
`:for i in range(1,100) | for j in range(6,10) | for k in range(i+1,100) | for l in range(6,10) | put = map(range(i,i), 'printf(''%03d'',v:val)')[0].'_'.map(range(j,j), 'printf(''%02d'', v:val)')[0].' '.map(range(k,k), 'printf(''%03d'',v:val)')[0].'_'.map(range(l,l), 'printf(''%02d'', v:val)')[0] | endfor|endfor|endfor|endfor`


