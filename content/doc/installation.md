---
title: "Installation"
weight: 1
# geekdocFlatSection: false
# geekdocToc: 6
# geekdocHidden: false
---

{{< tabs "uniqueid" >}}
    {{< tab "macOS" >}}
## Homebrew

```sh 
brew tap gravatalonga/ninja-lang
brew install ninja-lang
```
    {{< /tab >}}
    {{< tab "Linux" >}}
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
    {{< /tab >}}
    {{< tab "Windows" >}}
We are working to be available for [chocolatey](https://chocolatey.org/)  

But for the moment we have available via manual [installation](https://github.com/gravataLonga/ninja/releases). 

    {{< /tab >}}

    {{< tab "Manual">}}
## Manual Download

Download from [github](https://github.com/gravataLonga/ninja/releases)


## Source Code  

```bash    
git clone https://github.com/gravataLonga/ninja
cd ninja
go build -o ninja-lang
```   

    {{< /tab>}}
{{< /tabs >}}

