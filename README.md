## linux 
### main command 
  - `lsof` : list of processes that may be using the files .**ex**:`sudo lsof /var/lib/dpkg/lock-frontend` 
#### 1. set new password
```
sudo passwd root
```
#### 2. if APT package index can often become outdated as the packages or `sudo apt-get update` is error and interrupt :
###### before follow code below please check networking (if use vmware) or virual machine
```shell
sudo rm -rf /var/lib/apt/lists/*
sudo apt-get update
```
> if above not solve :
> ```shell
> sudo rm -R /var/lib/apt/lists/partial/*
> sudo apt-get update
> ```
#### 3 list port listen
```shell
sudo lsof -i -P -n | grep LISTEN
```
