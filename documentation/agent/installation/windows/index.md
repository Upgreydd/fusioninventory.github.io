---
layout: page
title: Microsoft Windows installation for agent Agent 2.3.x
redirect_from:
 - /documentation/agent/installation/windows.html
---

# Microsoft Windows Installation

{% include warning.html param="The new FusionInventory Agent 2.3.x comes with a **new** Microsoft Windows installer. The documentation you have below concerns this new installer. If you are looking for documentation on FusionInventory Agent 2.2.x (or earlier) and its installer, see link." %}
You can find [documentation on FusionInventory Agent 2.2.x]({{ site.baseurl }}/documentation/agent/installation/windows_before_2.3.0.html).


## Get the Installer



You can get the last FusionInventory Agent installer for Microsoft Windows [here](http://forge.fusioninventory.org/projects/fusioninventory-agent-windows-installer/files "http://forge.fusioninventory.org/projects/fusioninventory-agent-windows-installer/files"). The filename of the installer follows this pattern:



    fusioninventory-agent_windows-<platform>_<version>.exe
                                       |         |
                                       v         |
                                                 |
                                 'x86' | 'x64'   |
                                                 v
                                                  
                     <major>.<minor>.<release>[-<package>]



Some notes about the new FusionInventory Agent installer for Microsoft Windows.



* The installer for each *\<platform>*, integrates its native, although reduced, version of [Strawberry Perl](http://strawberryperl.com/ "http://strawberryperl.com/") 5.18.1.1.



* Inside the *\<version>*, *\<package>* is optional and indicates the secuence of the installer for FusionInventory Agent *\<major>*.*\<minor>*.*\<release>*. A new *\<package>* may contain improvements regarding the installer itself, the agent (patches) or both.



* It's possible to install *fusioninventory-agent_windows_x86_\<version>.exe* on a 32-bit or 64-bit Microsoft Windows system but it's only possible to install *fusioninventory-agent_windows_x64_\<version>.exe* on a 64-bit Microsoft Windows system.



## The Installer Manual



You can find the manual of the FusionInventory Agent installer for Microsoft Windows [here]({{ site.baseurl }}/documentation/agent/installation/windows/windows-installer-2.3.x-command-line.html).



The manual is contained within the installer. You can get it in one of the following ways:



*         C:\> fusioninventory-agent_windows-<platform>_<version>.exe /help



*         C:\> fusioninventory-agent_windows-<platform>_<version>.exe /dumphelp



*         C:\> fusioninventory-agent_windows-<platform>_<version>.exe /dumphelp /S


{% include info.html param="It's recommended that you read through this documentation each time a new version is released; the new FusionInventory Agent installer for Microsoft Windows is still young and it's in constant development, including its manual." %}


## Installation from Command Line and Silent Installation



The FusionInventory Agent installer for Microsoft Windows performs a *visual mode* installation unless you specify the ***/S*** option on the command line, in which case a *silent mode* installation is performed.



For more information about the use of the command line, please, see ***The Installer Manual*** section above.



## Visual Installation



As stated above, if the FusionInventory Agent installer for MS Windows is run without the ***/S*** option, it runs a *visual mode* installation. The easiest way to perform a *visual mode* installation is double-clicking on the *fusioninventory-agent_windows-\<platform>_\<version>.exe* file.



The fields and controls that appear in the *visual mode* installation are strictly related to the command line options. For that reason it's recommended that you read ***The Installer Manual*** section above before proceeding with the installation.



For more information about the *visual mode* installation, please, see the following gallery of [commented screenshots of FusionInventory Agent installer for Microsoft Windows]({{ site.baseurl }}/documentation/agent/installation/windows/windows-installer-2.3.x-visual-mode.html). (*still under construction*)



## Large Installations



There's a page dedicated to explaining [how to deploy FusionInventory Agent 2.2.x (or earlier) on a Windows Domain]({{ site.baseurl }}/documentation/agent/installation/windows/large_install.html) but, at the moment, its instructions are not valid for the new FusionInventory Agent installer.



For the time being, until the new page gets updated with more details, a new VBScript (Visual Basic Script) has been made available to allow you to perform an unattended deployment of *fusioninventory-agent_windows-\<platform>_\<version>.exe* in large (and in not so large) environments. The script is named *fusioninventory-agent-deployment.vbs* and it lastest version can be found [here](https://raw.github.com/fusinv/fusioninventory-agent/2.3.x/contrib/windows/fusioninventory-agent-deployment.vbs "https://raw.github.com/fusinv/fusioninventory-agent/2.3.x/contrib/windows/fusioninventory-agent-deployment.vbs").



## Installation from Sources



If you are a developer, or an advanced user, you can also install FusionInventory Agent 2.3.x [from sources]({{ site.baseurl }}/documentation/agent/dev/git_windows.html).



