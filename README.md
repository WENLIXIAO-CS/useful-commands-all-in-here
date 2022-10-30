# useful-commands-all-in-here
useful ubuntu / remote server / machine learning / .... commands

# Ubuntu
```
# Add ssh key to remote server
ssh-copy-id user@host

# How to see detailed information about a given PID?
ps -Flww -p THE_PID

# Grand sudo privileges to user
sudo usermod -a -G sudo username

# Remove sudo privileges from user
sudo deluser username sudo

# Recursively change access permission
chmod -R ug+rw foldername

```

### Check all python processes
```
ps -ef | grep python
```

## git / github

### Add server's ssh key to github
```
ssh-keygen -t ed25519 -C "randyxiao@email.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
cat ~/.ssh/id_ed25519.pub
```


### remove cache
```
git rm -r --cached .
```

## Jupyter Notebook

### Auto Reload
```
%load_ext autoreload
%autoreload 2
```

