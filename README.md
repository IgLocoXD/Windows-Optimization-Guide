# Windows Optimization Guide 

***I recommend you to use the HTML version of this guide, take me now!***

Windows despite being the operating system with the largest market share in the world does not make it the most "light" for everyone, it is understandable, since it is focused on so many end users with many different needs and a lot of hardware, **it's hard for everyone to have a good experience**.

I created this small repository with some extra files (which I will explain what each of them are for) to make a simple guide to optimize windows to the maximum

---

⚠ ***90% OF THE SCRIPTS ARE MADE BY OTHER PEOPLE***

I will just give a simple explanation of what each of these do, how to use them and other extra stuff.

I will also give credit to each person and links to the repositories.

---

# Contents

1) [Download Windows 10](#getWin10)

## Before you start

I will assume you are on a fresh installation of windows, it is the most recommended if you want a functional and practically garbage free system, I would personally recommend to do it at least once a year.

<h3 id="getWin10">Obtain Windows 10 ISOs</h3>

There are several ways to obtain ISOs of Windows 10 and also quite simple.

1) <a id="getWin10M1"> [Official (Slow)](https://www.microsoft.com/en-us/software-download/windows10) </a>: Downloading the system update tool to get the latest version of the system (This will download a system update download tool, a bit slow compared to the next way).
2) [Official (Faster?)](https://www.microsoft.com/en-us/software-download/windows10): Now instead of using the above tool we will download an ISO directly from the site, just follow a few steps to start with

    a) Depending on your browser, use the following key combination to open the developer tools, in my case (Chrome), I have to use the combination `Ctrl + Shift + I`
    
    b) Now `Ctrl + Shift + M` to activate the device toolbar, so our browser will make the page think that we are on a phone, finally press `F5` to refresh the page. If this doesn't work for your browser I recommend searching for `set user agent in <<your browser>>`
    
    c) After the page refreshes you will see a type of form you have to choose simple information.
    
    1) Multi-Edition ISO
    
    2) Your preferred language
    
    3) Your CPU architecture: An easy way to know what is the architecture of your PC; open your CMD and type `wmic OS get OSarchitecture`, this will show you your architecture.

3) [Universal Media Creation Tool](https://github.com/AveYo/MediaCreationTool.bat): Universal Media Creation Tool is a script made in Batch and PowerShell that allows you to download any version of windows 10, even the enterprise editions, it's very useful. It also downloads everything from official windows servers, the problem is that like [method 1](#getWin10M1) it uses a download tool which can be a bit more annoying than a direct download.

4) [Windows Downloader](https://www.heidoc.net/joomla/technology-science/microsoft/67-microsoft-windows-and-office-iso-download-tool): This program not only allows you to download Win10 ISOs but also lets you download Office directly. But to be honest I have never used it, I just know it exists.

    
⚠ ***Personally I think it is a bad idea to download the latest version of the system because in Windows 10 the newer the version the heavier the ISO is, the longer it takes to install, IT IS MUCH SLOWER. Unless you want to make sure you use a newer and therefore more secure version. Otherwise, and you really want maximum performance, I would recommend version 1903.***
