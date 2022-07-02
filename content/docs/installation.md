---
title: "Installation"
weight: 1
# geekdocFlatSection: false
# geekdocToc: 6
# geekdocHidden: false
---

## Homebrew  

```sh 
brew tap gravatalonga/ninja-lang
brew install ninja-lang
```

## Rpm / Yum  

To enable, add the following file `/etc/yum.repos.d/fury.repo`:  

```ini 
[fury]
name=Gemfury Private Repo
baseurl=https://yum.fury.io/gravatalonga/
enabled=1
gpgcheck=0 
```  
Check if correctly created `yum --disablerepo=* --enablerepo=fury list available`  

To install you only need run following command:  
```sh
yum install ninja-lang  
```

## APT  

To configure apt access, create a following file `/etc/apt/sources.list.d/fury.list` with content of :

```ini 
deb [trusted=yes] https://apt.fury.io/gravatalonga/ /
```  

Or use this one line command:

```bash 
echo "deb [trusted=yes] https://apt.fury.io/gravatalonga/ /" > /etc/apt/sources.list.d/fury.list
```  

and them you can install

```bash  
sudo apt install ninja-lang
```  

## Manual Download  

Download from [github](https://github.com/gravataLonga/ninja/releases)


## Manual Installation  

```bash    
git clone https://github.com/gravataLonga/ninja
cd ninja
go build -o ninja-lang
```   
