# novaha-bro-training #

# Bro Crash Course #
#### Facilitors: ####
    Liam Randall <Liam@Bro.org>
    Scott Runnels <srunnels@gmail.com>

## Prerequisites ##
### SecurityOnion ###
    
A copy of SecurityOnion installed into a VM.  Simply install it; you do not need to run the "Setup" wizard and actually enable the SO Suite of tools for active usage.
    
If you are using VMWare please also install VMWare Tools into your new SecurityOnion VM; if VirtualBox please make sure to install the Guest Additions.

    
### Git Hub ###
    
If you do not already have a github account, please take the time to create one now.  For the class we will be cloning repositories for configuration demonstrations, customization examples, and programming demo's.  You can quickly install Git onto your SO Box with:
    
    sudo apt-get install git
    
From there please follow the following steps to create your git account, create your first test repo, and then fork a sample repo:
    
    https://help.github.com/articles/set-up-git
    https://help.github.com/articles/create-a-repo
    https://help.github.com/articles/fork-a-repo

    
    
## Bro Introduction ##

Install the demonstrationss for today

	git clone git://github.com:LiamRandall/bro-scripts.git bro-scripts
	git clone git://github.com:LiamRandall/novaha-bro-training.git novaha-bro-training

Overview

## Setup Your Development Environment ##

[sublime2]: http://liamrandall.com/syntax-highlighting-for-bro-network-programming-language/ "Setup Sublime 2"

[Setup Sublime-2 with Syntax Highlighting][sublime2]

Download Sublime:

	http://www.sublimetext.com/2
	tar -xvjpf Sublime Text 2.0.1 x64.tar.bz2
Go ahead and start Sublime for the first time:

	cd Sublime Text 2/
	./sublime_text to launch

Enter the Sublime control window with the shortcut CONTROL+TICK; the tick: ` is in the top left corner under the tilda: ~:

	ctrl+`
Install package control window just cut and paste the following:

	import urllib2,os; pf='Package Control.sublime-package'; ipp=sublime.installed_packages_path(); os.makedirs(ipp) if not os.path.exists(ipp) else None; urllib2.install_opener(urllib2.build_opener(urllib2.ProxyHandler())); open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read()); print 'Please restart Sublime Text to finish installation'



## Bro Basics ##


## Bro Customization Points ##




Install the Bro APT1 Report Module:


	sudo apt-get install -y git
	cd /opt/bro/share/bro/site/
	sudo git clone git://github.com/sethhall/bro-apt1.git apt1
	echo "@load apt1" | sudo tee -a local.bro



## Searching Logs ##

    

## Scripting Approach ##
#### Overview ####



## Programming Examples ##

### HTTP Bruteforcing ###
#### Overview ####


#### Count All the Things ####


#### Notice Framework: Cluster Safe Logging ####



#### Problem Approach ####


#### Metrics Framework: Cluster Safe Couting ####



