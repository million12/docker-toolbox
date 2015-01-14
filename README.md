##CoreOS Toolbox replacement
This is a [million12/toolbox](https://registry.hub.docker.com/u/million12/toolbox/) docker container with CoreOS toolbox replacement. It is based on CentOS 7 and it's very lightweight, only ~293M (vs. 374M Official CoreOS Fedora). There are some basic tools already installed and ready to use.  
### List of installed tools  
`htop`  `atop`  `nmap`  `iftop`  `iotop`  `mc`  `net-tools`  `xfstools`

### Replace default CoreOS Fedora toolbox  
Add file `.toolboxrc` into your user home directory with this content:  
`vi ~/.toolboxrc`  

`TOOLBOX_DOCKER_IMAGE=million12/toolbox`  
`TOOLBOX_USER=root`  

### Usage examples 
You can use a name of tool as a parameter when running toolbox  

`toolbox htop`	Will run htop  
`toolbox atop` Will un atop  
...  

**Note:** First run might take a little while as the image need to be pulled from docker hub repository server. Every other `toolbox command` will work straight away.


## Author(s)

* Przemyslaw Ozgo (<linux@ozgo.info>)

---

**Sponsored by** [Typostrap.io - the new prototyping tool](http://typostrap.io/) for building highly-interactive prototypes of your website or web app. Built on top of TYPO3 Neos CMS and Zurb Foundation framework.
