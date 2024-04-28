<h1 align="center">
  The Abstrakt Project Repository
  <br>
</h1>

<h4 align="center">Abstrakt is a system-level application designed to target, kill and remove a running process by name. Useful for large-scale operations in certain work environments.</h4>

<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#installation">Installation</a> •
  <a href="#download">Download</a> •
  <a href="#issues-and-contributing">Issues and Contributing</a> •
  <a href="#disclaimer">Disclaimer</a>
</p>


## Key Features

* Local "Beacon" Server 
  - A beacon-server script that Abstrakt will communicate with to receive updates, commands or other information.
* Silent Background operation 
  - Customizable with various options including a `no-console` launcher that compiles and runs the script quietly until forcefully terminated by Host or `!kill` command or equivalent is issued from Beacon.
* Lightwork, and clock-work
  - Goes easy on hardware that isn't too powerful thanks to it's IRPV algorithm, Intelligent Resource Provisioner, that actively checks hardware resource usage and adjusts its own depending on instructions from Beacon or task-kill list parameters.
* Sleeper-mode^
  - Script can change its behavior to avoid detection some include ceasing log-file creations, changing its process name, creating a setup/helper script that will respawn Abstrakt after its removal, or spawn `guard-dog` instances.
  - Special thanks to our hardworking watch-dogs for this one, as they are restlessly watching Abstrakt and restarting it upon termination and reporting back incident to Beacon.
<br></br>
  > `Guard-dog` instances are scripts that attempt to evade system process-kill by using various methods, customizable with Beacon.
  > Note that, in this context, `Guard-dogs` are not related to `watch-dogs`.

* Custom Timeout interval 
  - Processes restarting too fast? Not a problem. You can adjust the timeout check-interval to check more often. or you 
* Whitelists and Blacklists
  - Know who's friend and who's foe? Send out `whitelist.json` and `blacklist.json` files from the Beacon and Abstrakt will take care of the rest.
  - Don't which process is critical? Abstrakt can fetch a list of all currently running processes and send it back to Beacon. You can then manually whitelist running processes, such as system processes and Abstrakt itself, and blacklist the rest or configure the Beacon to automatically do that instead, if it suits your needs.
  - Option to export the process list locally as `.txt` or send it to Beacon as `.json` within a pre-specified interval.
* Supports Group Mode* 
  - Group mode makes it possible for Abstrakt to run simultaneously with other Abstrakt instances and won't terminate them. To activate it, simply send a command from the Beacon.
* Options for Exporting the running processes list
  - Option to export the process list locally as `.txt` or send it to Beacon as `.json`.

  > ^ Log files are always sent back to Beacon regardless of this setting. 
  > Beacon-server, sleeper-mode, task-kill list, multiple instances, advanced IRPV configuration and certain other features may only be available to `Abstrakt Pro` releases.


## Installation
 
<h3>Run compiled source</br></h3>

> Python3 is required to be installed on your system before proceeding. 

```bash
# Clone this repository
$ git clone https://github.com/Team12RunnersLLC/Abstrakt.git

# Go to dir of setup wizard
$ cd Abstrakt/compile

# Run setup wizard `setup.pyw`
$ python setup.pyw

# Run abstrakt 
$ abstrakt.exe
```
<em> To use `no-console` mode, rename `abstrakt.py` --> `abstrakt.pyw` before running setup wizard `setup.pyw` </em>

<h3>Run from source</br></h3>

> Python3 & all imports in `requirements.txt` are required to be installed on your system before proceeding.

```bash
# Clone or Download source `abstrakt.py` file from repo
$ git clone https://github.com/Team12RunnersLLC/Abstrakt

# Download required packages from `requirements.txt`
$ pip install -r requirements.txt

# Run `abstrakt.py` or `abstrakt.pyw` for no-console mode
$ python abstrakt.py
```


## Download

This link points to the [latest version](https://github.com/Team12RunnersLLC/Abstrakt.git) of Abstrakt for Windows.


## Issues and Contributing

We encourage you to read our [issues guide](https://github.com/Team12RunnersLLC/Abstrackt/issue-reporting.md) before reporting any issues.
If you would like to contribute to this project, we ask that you familiarize yourself with our workflow by reading the [contribution guide](https://github.com/Team12RunnersLLC/Astrakt/contribute.md) first to help you get started.


## Disclaimer

* [[Github]](https://github.com/Team12RunnersLLC) 
* [[Website]](https://t12r.pythonanywhere.com/) </br>


> Some parts of this repository contain code that may not be owned or created by the developers of Demand, Team12Runners LLC, or T12R Inc.</br>
>
> Redistribution of any part of this repository in any way shall have this disclaimer section explicitly written in all files taken from this repository by the owners, creators, founders or maintainers of that repository.</br>


###### <em> © 2024 Team12Runners LLC, T12R Inc. All Rights Reserved. Property protected under Copyright Law.</em>
