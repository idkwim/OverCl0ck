## OverCl0ck

A (currently) early prototype concept for an Apple Watch Jailbreak. Uses the v0rtex kernel exploit, and therefore supports watchOS3. Exactly compatbility across OS versions and hardware is unknown. Most things are unknown.

Offsets can be found using my fork of tihmstar's offsetfinder, [watch_offsetfinder](https://github.com/PsychoTea/watch_offsetfinder).

To enable proper NSLog functionality you may need to use [this](http://dl.sparko.me/watchOSlogging.mobileconfig) provisioning profile (make sure to install it to your Apple Watch, not your iPhone)

I'm unsure if v0rtex even runs as-is - the process of finding offsets still needs work.

Feel free to play around with this and let me know if you find anything interesting.

Post-exploitation shouldn't be too difficult, as the Watch is 32bit, therefore no KPP.

**Please remember to work from the 'develop' branch, and submit PR's there. NOT master.**

To-do:
- Fix watch_offsetfinder to correctly find sizeof_task and iouserclient_ipc
- Get v0rtex to run correctly
- Patch the shit out of the kernel
- Disable codesigning
- Mount '/' as r/w
- Spawn dropbear/shell

In the future:
- Find reliable way to transfer files to Watch
- Subtitute port to watchOS
- Full package manager for Watch tweaks
- Get dough

These resources may provide useful:

https://www.youtube.com/watch?v=eJpbi-Qz6Jc

https://speakerdeck.com/mbazaliy/jailbreaking-apple-watch-1

https://speakerdeck.com/mbazaliy/jailbreaking-apple-watch

RIP Apple Watch, April 2015 - January 2018 💀
