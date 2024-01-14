---
layout: post
title:  "How to install Windows"
categories: misc
comments: true
---
Hello everyone. Today I will show you how to install Windows. Unironically. Let me know if you had any TILs or if you think I missed something. This is how I setup my Windows.

Windows machines need to be cleaned every now and then due to how it's built, unlike GNU. My reason today was not however a routine formatting of the C drive. Finland's worst [bofferer](https://en.wikipedia.org/wiki/Foam_weapon), my friend just bought a 2tb nvme m.2 ssd. My setup so far has been os on nvm2, games and software on sata ssd and important/large files on hdd. I got tempted by satan and bought a pcie gen4 nvme 2tb ssd. Because nvme m.2 uses four lanes of pcie i just got a speed boost of around 2x so my nvme is around 8gbps fast. The amount of hentai i will transfer from my pc to my oculust quest 2 will be immaculate.

After making my usb stick bootable with the help of windows installation assistant I started installing it. Apparently Windows N and KN versions mean (maybe) "No multimedia" and "Korea No multimedia".

> These editions of Windows exist entirely for legal reasons. In 2004, the European Commission found Microsoft had violated European antitrust law, abusing its monopoly in the market to hurt competing video and audio applications. The EU fined Microsoft €500 million and required Microsoft to offer a version of Windows without Windows Media Player. Consumers and PC manufacturers can choose this version of Windows and install their preferred multimedia applications without Windows Media Player also being present. It's not the only version of Windows offered in the European Union---it's just an option that has to be available. This is why the "N" editions are only available in Europe.

Also it turns out choosing a name for your PC is as difficult as choosing your starter Pokémon. I will go with Stallmachine.

![richard stallman sleeping](/assets/stallman.jpg)

I thought the installation would take as long when it 15 years ago on my Windows 7. I wasn't expecting an all-nighter but at least a few minutes. For this I bought Jany Austen's Pride and Prejudice. Look at how lovely the cover made by [Elina Warsta](https://solmu.nu/) is!!!

![Pride and Prejudice cover](/assets/pride.png)

I read it for a few minutes then I got reminded of the 8gbps speed of my new nvme. The thing had already finished.

Allow all tracking and dev logs because sustainability. Reminder for myself to change my insecure Microsoft and Google passwords to something longer and more easily typable. Apparently I've set 1600 dpi to my mouse's internal memory so luckily it stayed that way.

We're now inside Windows 11. Install Chrome. Nice to know that Edge doesn't edge anymore how one should stay with Edge when trying to download Chrome.

Set dark theme because [sustainability](https://dl.acm.org/doi/pdf/10.1145/3458864.3467682) and [inclusivity](https://www.kinandcarta.com/en/insights/2023/09/does-dark-mode-win-on-sustainability-and-accessibility/) reasons. Install Geforce Experience and drivers from mobo manufacturer site. Clean up taskbar. Remove bloat software. Enable autologon from sysinternals. Install 7-zip because autologon was zipped because I was taught in a malware analysis and reverse engineering class that Windows' unzipper works with Windows Defender so it might be lossy. Remove autosearch from Windows search into Edge. Use these registry scripts I crafted if you want to. Uninstall script provided as well if it doesn't work out for you.

[DisableSearchBoxSuggestions](/assets/disableSearchBoxSuggestions.reg)

[removeDisableSearchBoxSuggestions](/assets/removeDisableSearchBoxSuggestions.reg)

Wtf mouse acceleration is on by default. Disable it. Screensaver time is apparently very short. Blacken screen in 5 hours. Suspend never due to torrent reasons. Create symlinks from my home to my harddrive with powershell so that, eh never mind maybe I'll just show what I've done so you understand what I've done.

{% highlight powershell %}
New-Item -ItemType SymbolicLink -Path ".\Musiikki\" -Target "D:\Musiikki\";`
New-Item -ItemType SymbolicLink -Path ".\Kuvat\" -Target "D:\Kuvat\";`
New-Item -ItemType SymbolicLink -Path ".\Videot\" -Target "D:\Videot\";`
New-Item -ItemType SymbolicLink -Path ".\Tiedostot\" -Target "D:\Tiedostot\";
{% endhighlight %}

![windows home folder symlinks](/assets/homefolders.png)

One blue screen later my Windows 11 basic installation is now finished. I will install lots of bloat like [SoundSwitch](https://soundswitch.aaflalo.me/), emulators, programming tools and what not but this is what peak Windows looks like.

![Windows desktop](/assets/windows.png)

Did I miss anything? Lemme know.
