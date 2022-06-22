# Basic-Software-Installation-for-Particle-Physics

This page is the guidance for newcomers to install some software, which is essential for further simulation jobs in particle physics.

## WSL2 (Linux subsystem for Windows 10)
**Linux on Virtual Machine like VirtualBox or VMWare is not recommended.**\
Automatic Installation [Click Here](https://docs.microsoft.com/zh-cn/windows/wsl/install)  
When some problems occur with automatic installation or you want to customize the Linux version, please choose:\
Manual Installation [Click Here](https://docs.microsoft.com/zh-cn/windows/wsl/install-manual)

## MobaXterm
A very useful tool for **Windows 10 users** to connect WSL and SJTU bl-0 server. It also provides visualization , which is necessary when drawing plots. Unnecessary for Macbook users \
Official webpage [Click Here](https://mobaxterm.mobatek.net/)

## VScode
A quite powerful tool for code editing on both WSL and bl-0 server. Its only shoutcoming is that it does not support visualization. Strongly recommended for all to install.\
Official webpage [Click Here](https://code.visualstudio.com/)\
Tutorial for WSL2 setup in VScode [Click Here](https://docs.microsoft.com/en-us/windows/wsl/tutorials/wsl-vscode)\
Tutorial for SSH Server setup (connet bl-0 server) [Click Here](https://code.visualstudio.com/docs/remote/ssh)

## CLion (Optional)
Another powerful tool to operate C/C++ based project. It also supports WSL and SSH server. Although until now I've not successfully connect to bl-0 server on Windows 10, it is worth trying. It works quite well in WSL.\
Official webpage [Click Here](https://www.jetbrains.com/clion/)\
You can use it free of charge as long as you get the individual license for students with your education e-mail. It need to be refreshed every year. [Click Here](https://www.jetbrains.com/community/education/#students)\
Tutorial for WSL setup [Click Here](https://www.jetbrains.com/help/clion/how-to-use-wsl-development-environment-in-product.html#wsl-tooclhain)\
Tutorial for SSH Server setup (A little bit complex) [Click Here](https://www.jetbrains.com/help/clion/remote-projects-support.html#excluded-paths)

## ROOT
An indispensable software for data analysis in particle physics.\
Official webpage [Click Here](https://root.cern/)\
Installation tutorial [Click Here](https://root.cern/install/)\
Build from source guide. Quote from webpage: ```In case no other installation method is available, or if you want full control over the options ROOT is built with, it is possible to compile ROOT from source.``` **Build from souce is recommended since it enables customization and the following installation of Geant4 and musrSim can follow the same process.** [Click Here](https://root.cern/install/build_from_source/)

ROOT Topical Manual. It provides basic operation tutorial in detail for some most commonly used classes such as Histogram or Tree. This manual is quite handy for daliy use and reference. [Click Here](https://root.cern/topical/)\
For further reference, use ROOT Reference Guide, which is a bit prolix and esoteric. [Click Here](https://root.cern/doc/master/)

## Geant 4
Another indispensable simulation framework for particle physics.\
Getting Started page [Click Here](https://geant4.web.cern.ch/support/getting_started)\
Download Source Code [Click Here](https://geant4.web.cern.ch/support/download)\
Building and Installing from Source Guide [Click Here](https://geant4-userdoc.web.cern.ch/UsersGuides/InstallationGuide/html/installguide.html#buildandinstall)\
Geant 4 build options. If customization is needed, these options should be specified along with CMake options [Click Here](https://geant4-userdoc.web.cern.ch/UsersGuides/InstallationGuide/html/installguide.html#geant4buildoptions)

## musrSim
A simulation software based on Geant 4 and ROOT.\
Source code [Click Here](https://www.psi.ch/en/lmu/geant4-simulations#source-code-of-musrsim)\
Installation: Follow the same process as building and installing from source code of ROOT and Geant 4. 
