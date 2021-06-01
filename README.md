## linux 
####1. set new password
```
sudo passwd root
```
####2. if APT package index can often become outdated as the packages or **sudo apt-get update** is error and interrupt :
```
sudo rm -rf /var/lib/apt/lists/*
sudo apt-get update
```
> if above not solve :
> ```
> sudo rm -R /var/lib/apt/lists/partial/*
> sudo apt-get update
> ```

