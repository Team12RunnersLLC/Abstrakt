
<h1 align="center">
  The Abstrakt Project 
  <br>
</h1>

<h4 align="center">Demand is a multi-feature, system-level command line interface (CLI). Includes built-in ssh, or uses Host's ssh, network discovery, dns & rdns lookup, zap and nmap assisted scanning and more!</h4>

<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#download">Download</a> •
  <a href="#credits">Credits</a> •
  <a href="#related">Related</a> •
  <a href="#license">License</a>
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


## How To Use

 <h4>There are two ways to use Abstrakt: </h4>
 
* Clone this repository, then compile and run it
> Python3 & all imports in `requirements.txt` are required to be installed on your system before proceeding. 
- Clone this repository and run `setup.exe` to compile this application or download the source `.py` file and run it, you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
$ git clone https://github.com/blinkyboi/Demand

# Go into the repository
$ cd electron-markdownify

# Install dependencies
$ npm install

# Run the app
$ npm start
```

> **Note**
> If you're using Linux Bash for Windows, [see this guide](https://www.howtogeek.com/261575/how-to-run-graphical-linux-desktop-applications-from-windows-10s-bash-shell/) or use `node` from the command prompt.


* Dowload the source `.py` file and run it


## Download

You can [download](https://github.com/amitmerchant1990/electron-markdownify/releases/tag/v1.2.0) the latest installable version of Markdownify for Windows, macOS and Linux.

## Emailware

Markdownify is an [emailware](https://en.wiktionary.org/wiki/emailware). Meaning, if you liked using this app or it has helped you in any way, I'd like you send me an email at <bullredeyes@gmail.com> about anything you'd want to say about this software. I'd really appreciate it!

## Credits

This software uses the following open source packages:

- [Electron](http://electron.atom.io/)
- [Node.js](https://nodejs.org/)
- [Marked - a markdown parser](https://github.com/chjj/marked)
- [showdown](http://showdownjs.github.io/showdown/)
- [CodeMirror](http://codemirror.net/)
- Emojis are taken from [here](https://github.com/arvida/emoji-cheat-sheet.com)
- [highlight.js](https://highlightjs.org/)

## Related

[markdownify-web](https://github.com/amitmerchant1990/markdownify-web) - Web version of Markdownify

## Support

<a href="https://www.buymeacoffee.com/5Zn8Xh3l9" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>

<p>Or</p> 

<a href="https://www.patreon.com/amitmerchant">
	<img src="https://c5.patreon.com/external/logo/become_a_patron_button@2x.png" width="160">
</a>

## You may also like...

- [Pomolectron](https://github.com/amitmerchant1990/pomolectron) - A pomodoro app
- [Correo](https://github.com/amitmerchant1990/correo) - A menubar/taskbar Gmail App for Windows and macOS

## License

MIT

---

> [amitmerchant.com](https://www.amitmerchant.com) &nbsp;&middot;&nbsp;
> GitHub [@amitmerchant1990](https://github.com/amitmerchant1990) &nbsp;&middot;&nbsp;
> Twitter [@amit_merchant](https://twitter.com/amit_merchant)












> Some parts of this repository contain code that may not be owned or created by the developers of Demand, Team12Runners LLC, or T12R Inc.
> Redistribution of any part of this repository in any way without explicit written consent from the owners, creators, founders or maintainers of this repository is prohibited and is protected under Copyright Law.
</br> <> (C) 2024 Team12Runners LLC, T12R Inc.  |  All Rights Reserved </> 
