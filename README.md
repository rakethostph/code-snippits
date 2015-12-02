# Assorted Snippits

**Hack any paid WiFi hotspot in about 30 seconds**
```
ifconfig en1 | grep ether
arp -a
sudo ifconfig en1 ether [mac address to spoof]
```

# Git Command

* `git init` creates a new Git repository
* `git status` inspects the contents of the working directory and staging area
* `git add` adds files from the working directory to the staging area
* `git diff` shows the difference between the working directory and the staging area
* `git commit` permanently stores file changes from the staging area in the repository
* `git log` shows a list of all previous commits

