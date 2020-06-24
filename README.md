# Development Environment and Vagrant 101

#### What is an Environment?

#### Dev Environment

#### 4 Pillars of DevOps

#### DevOps problems and solutions


## Vagrant & Virtual Box

### Virtual Box

### Vagrant


### Package Managers

#### What is a package manager?
A package manager is a collection of software tools that automates the process of installing, upgrading, configuring, and removing computer programs for a computer's operating system in a consistent manner.

#### What is pythons package manager?
Pip is python’s package manager. It has come built-in to Python for quite a while now, so if you have Python, you likely have pip installed already.

#### What about other languages?
RubyGems for (Ruby)
Packagist for (PHP)
NPM for (Node. JS)
Bower for (JS, CSS, HTML)
CocoaPods for (Objective-C)
Maven for (Java)

#### what are package managers for windows and mac?
Mac: Macs do not have a main included package manager.
- Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple's macOS operating system and Linux.

Windows: Chocolatey is more comparable to brew on Mac, but it is a great way to keep track of the packages you have and which version of that package you are on.

#### what is the package manager for Ubuntu? 
The default package manager for Ubuntu is apt-get.

# Vagrant

### What goes on the vagrant file?

1. config.vm.box | This is our Operating System! We will be using ubuntu 64 bit
2. config.vm.provider | This is VirtualBox
3. config.vm.network | How your host computer sees your box
4. config.vm.synced_folder | How you access files from your computer
5. config.vm.provision | What do we want to run as a provision for shell commands. What dependencies are needed? Node js? nginx?
If we dont use provisions, Vagrant will just run a blank ubuntu server

### Commands

1. vagrant init | Initiates Vagrant 
2. vagrant up | Activates Vagrant file and runs Virtual machine
3. vagrant suspends | Saves the virtual machine and suspend it / make it offline
4. vagrant resume | Resumes the virtual machine
5. vagrant destroy | Destroys the virtual machine
