# Personal Windows Optimization Guide 

***Working on a HTML version***

Windows despite being the operating system with the largest market share in the world does not make it the most "light" for everyone, it is understandable, since it is focused on so many end users with many different needs and a lot of hardware, **it's hard for everyone to have a good experience**.

I created this small repository with some extra files (which I will explain what each of them are for) to make a simple guide to optimize windows to the maximum.

---

⚠ ***SCRIPTS MADE BY THIRD PARTIES***

Most of the scripts are made by other people.

I will just give a simple explanation of what each of these do, how to use them and other extra stuff.

I will also give credit to each person and links to the repositories.

---

## Contents

1) [Download Windows 10](#getWin10)
2) [Create a bootable pen drive](#bootUSB)
3) [Booting the system](#bootWin)
4) [Scripts and post-installation programs](#postInstall)
5) [Basic programs](#basicPrograms)

##### Extra

1) [Using a windows mod](#winMod)
2) [Time to use linux?](#linTim)

### Before you start

I will assume you are on a fresh installation of windows, it is the most recommended if you want a functional and practically garbage free system, I would personally recommend to do it at least once a year.

<h2 id="getWin10">Download Windows 10</h2>

There are several ways to obtain ISOs of Windows 10 and also quite simple.

1) [Official (Slow)](https://www.microsoft.com/en-us/software-download/windows10): Downloading the system update tool to get the latest version of the system (This will download a system update download tool, a bit slow compared to the next way).

2) [Official (Faster?)](https://www.microsoft.com/en-us/software-download/windows10): Now instead of using the update tool we will download an ISO directly from the site, just follow a few steps to start with.

    a) Depending on your browser, use the following key combination to open the developer tools, in my case (Chrome), I have to use the combination `Ctrl + Shift + I`
    
    b) Now use `Ctrl + Shift + M` to activate the device toolbar or click on the second icon in the upper left corner (it looks like a laptop with a phone), so our browser will make the page think that we are on a phone, finally press `F5` to refresh the page. If this doesn't work for your browser I recommend searching for `set user agent in <<your browser>>`
    
    c) After the page refreshes you will see a type of form you have to choose simple information.
    
    1) Multi-Edition ISO
    
    2) Your preferred language
    
    3) Your CPU architecture: An easy way to know what is the architecture of your PC; open your CMD and type `wmic OS get OSarchitecture`, this will show you your architecture.
    
    4) Finally this will download the ISO with the selected preferences, when the process is finished you can proceed [Booting the system] to install the system.

3) [Universal Media Creation Tool](https://github.com/AveYo/MediaCreationTool.bat): Universal Media Creation Tool is a script made in Batch and PowerShell that allows you to download any version of windows 10, even the enterprise editions, it's very useful. It also downloads everything from official windows servers, the problem is that like [method 1](#getWin10M1) it uses a download tool which can be a bit more annoying than a direct download.

4) [Windows Downloader](https://www.heidoc.net/joomla/technology-science/microsoft/67-microsoft-windows-and-office-iso-download-tool): This program not only allows you to download Win10 ISOs but also lets you download Office directly. But to be honest I have never used it, I just know it exists.

---
⚠ ***MORE RECENT MORE SLOWER***

Personally I think it is a bad idea to download the latest version of the system because in Windows 10 the newer the version the heavier the ISO is, the longer it takes to install, SO MUCH SLOWER IN GENERAL. Unless you want to make sure you use a newer and therefore more secure version. Otherwise, and you really want maximum performance, I would recommend version 1903.

Although well, I assume that if you see this repository is because you want a lightweight Windows and because probably your PC is not so powerful for the latest versions.

This [Wikipedia link](https://en.wikipedia.org/wiki/Windows_10_version_history) shows all Windows 10 versions highlighting if they are still supported or not.

---

<h2 id="bootUSB">Create a bootable pen drive</h2>

What is the best program to create a bootable USB? That question may depend on your tastes, I guess, so I made a (really) simple table to give you an idea of which one is the best.

| Tool                                           | Description                                                      | Easy to use?                                           | Open Source | Multi ISO | Windows | MacOS | Linux |
|------------------------------------------------|------------------------------------------------------------------|--------------------------------------------------------|-------------|-----------|---------|-------|-------|
| [Ventoy](https://www.ventoy.net/en/index.html) | An open-source tool to create bootable USB drives for ISO files. | 9/10 [Guide](https://www.ventoy.net/en/doc_start.html) | ✅           | ✅         | ✅       |       | ✅     |
| [Balena Etcher](https://etcher.balena.io/)     | A tool to create bootable USB drives from downloaded ISO files.  | 10/10                                                  | ✅           |           | ✅       | ✅     | ✅     |
| [Rufus](https://rufus.ie/en/)                  | A tool to create bootable USB drives from ISO files.             | 7/10                                                   | ✅           |           | ✅       |       |       |

Personally I recommend using Ventoy because it only requires copying the ISO file to the USB, it's that simple.

Also, in the table above there is an official user's guide.

<h2 id="bootWin">Booting the system</h2>

In this part I can't do an exact explanation of how to enter the BIOS of your PC, the most common is to use `F2`, `F10`, `F12`, `Del`, or even `Esc`. You can also search for `how to access the BIOS in <<your PC model>>`.

When you access it, find the section called `boot order`, modify the order so that the USB is in the first position. I would like to be more specific, but I can't.

Ah, yes... remember to save your changes.

What happens now will depend on whether you used [Ventoy](https://www.ventoy.net/en/index.html), [Balena Etcher](https://etcher.balena.io/) or [Rufus](https://rufus.ie/en/).

Finally, when you see this screen

*ins img*

go by what the interface says, it should be simple enough.
