---
layout: post
title: "Browsing safely"
date: 2019-05-16
last_modified_at: 2019-06-03
underconstruction: 'no'
---
This post describes how I have set up my computer and software for safety. My aim was to minimise my footprint on the Internet and make it more useable, most of the time. *This guide covers desktop and laptop computers, not tablets and phones.*

**Disclaimers:** Your mileage may vary. I am not a lawyer  (or a specialist in anything in particular). I don't work with anything  very secret (except my own personal information),. Do your own research, Don't blame me!

**Caution:** Some "clever" stuff on the Interweb will stop working on your  computer and/or in your browser. *That's the point!* -- lots of the "clever" stuff, especially scripts, is there to track you, show ads etc.

**Tradeoffs:** You'll have to do some work to set this up. Doing some things on the Internet will be a bit more  complicated. Buying things online, for example. Also, some very good  websites depend on advertising to cover their costs. Are you OK with  taking the bread from their mouths? If not, you are giving them and their  advertisers some (or a lot of) personal information. Some say, that's the price of  admission. Are you OK with that? As with so many things in life, you  must work out your own answers to questions like these. Also, some  security precautions will make your browser faster. (Not loading unwanted  content saves time.) But some of them will make it seem slower. (Not  prefetching linked pages before you click on the links means that the  browser only asks for the content when you actually click. But this  protects your personal information, because the add-on filters links that you click.)

# Basic setup

## Operating system

* **Windows** has nearly 90% of the installed base of desktops and laptops.[^1] If you're not on Windows 10, you should upgrade. Keeping up with all the security updates is a challenge, but it's not optional. The same applies to using Windows Defender for virus protection.

* If you have a **Mac**, chances are that you'll be using Apple's **macOS**. Mac users may be surprised to hear that Apple has less than 10% of the installed base. Keep macOS updated and upgraded and you'll mostly be OK. Antivirus software is available, but it may be overkill.

* Of the other operating systems, only **Linux** (2%) has more than 0.3%. Use a LTS (long-term support) version and update it regularly.

[^1]: February 2019 [(source)](https://en.wikipedia.org/wiki/Usage_share_of_operating_systems#Desktop_and_laptop_computers)

## Choosing a web browser

Browser options include:
* Google's Chrome (64%-72% share)[^2]
* Microsoft's Internet Explorer and Edge (together 7%-14%)
* Mozilla's Firefox (7%-9%)
* Apple's Safari (4%-14%)
* Chinese-owned Opera (2%-3%)
* Others (2%-6% combined)

[^2]: October/November 2018 [(source)](https://en.wikipedia.org/wiki/Usage_share_of_web_browsers#Summary_tables)

[**Firefox**](https://www.mozilla.org/firefox/new/) is my choice. It's not proprietary. Mozilla has no commercial axe to grind. It's open source and actively developed, with many available add-ons.

## Choosing a search engine

The next task is to avoid tracking of your searches. Google has 93% of the search market![^3] Microsoft's Bing and Yahoo! have most of the rest. DuckDuckGo gets a good press, but has irritating (to me) limitations. I use [**Startpage**](https://www.startpage.com).

[^3]: February 2019 [(source)](https://en.wikipedia.org/wiki/Web_search_engine#Market_share_in_February_2019)

When I can't avoid using a proprietary service, I routinely log out as soon as I finish using it. For example, I have to log into Google for a particular service that is not available elsewhere.

## Using browser add-ons to block unwanted content

My objective is to minimise the information that I give away when visiting websites. These free add-ons also speed up your browsing:
* [uBlock Origin](https://addons.mozilla.org/en-GB/firefox/addon/ublock-origin/) An efficient blocker of ads and other unwanted stuff. Also available for Chrome and Edge, and (possibly out-of-date) for Safari. By the excellent [Raymond Hill](https://github.com/gorhill).
* [Decentraleyes](https://addons.mozilla.org/en-GB/firefox/addon/decentraleyes/) Emulates Content Delivery Networks to improve online privacy [(details)](https://git.synz.io/Synzvato/decentraleyes/wikis/Simple-Introduction). Also available for Chrome and Opera.
* [uMatrix](https://addons.mozilla.org/en-GB/firefox/addon/ublock-origin/) A firewall that works in relaxed block-all/allow-exceptionally mode out-of-the-box. Some sites will break, so *this one is for advanced users*. Also available for Chrome and Opera. Also by [Raymond Hill](https://github.com/gorhill).

The first two of these can be used on an install-and-forget basis, but they are better with a little extra work. uMatrix requires more work, and it does more; as with all add-ons, you can always remove it if you don't like it.

## Configuring the add-ons

#### uBlock Origin

**Simplest way:** install and forget. Read [this](https://github.com/gorhill/uBlock/wiki/Quick-guide:-popup-user-interface). Short version: you can turn off uBO for the site you're looking at, and see it unmodified, at the cost of switching off its protection. uBO will remember your decision.

**Simple way:** in addition, consider [installing more filter lists](https://github.com/gorhill/uBlock/wiki/Dashboard:-Filter-lists).

**Expert way:** turn on uBO's [advanced user mode](https://github.com/gorhill/uBlock/wiki/Advanced-user-features) and use its full power.

#### Decentraleyes

There's no need to configure this. It can be turned off on a per-site basis, in the unlikely event that it breaks something.

#### uMatrix

*For experienced users.* Configuration is required, and you will do constant tweaking. [YouTube tutorial](https://www.youtube.com/watch?v=TVozpo3zUBk) 13m07s; [brief introduction with screenshots](https://www.ghacks.net/2017/11/28/a-umatrix-guide-for-firefox/); [author's wiki](https://github.com/gorhill/uMatrix/wiki)

## Other recommended add-ons

* [**Nano Defender**](https://addons.mozilla.org/en-GB/firefox/addon/nano-defender-firefox/?src=search), a supplement to uBlock Origin that overcomes some anti-adblocking measures used by websites. An easy install. [(documentation)](https://jspenguin2017.github.io/uBlockProtector/)

* [**HTTPS Everywhere**](https://addons.mozilla.org/en-GB/firefox/addon/https-everywhere/), which uses the more-secure http**s**:// version of websites, if available. Fit and forget.

## Firefox options and settings

Firefox has a huge list of settings that you can change. Here's [a good guide to privacy settings on Firefox](https://restoreprivacy.com/firefox-privacy/).

## While you're in the mood...

You probably know this already, but most virus infections start with clicking on a link in an email. It looks oh-so-plausible!

## Virtual Private Network (VPN)

Unlike the other recommendations here, VPNs are *not* free. Why would you want one? A VPN enables you to:
* Hide your real location when online, giving you extra anonymity
* Protect your privacy on untrustworthy wireless hotspots
* Overcome geographic restrictions on websites and video/audio providers, like Netflix and Hulu
* Avoid being logged when using torrents

Most people who use VPNs are pretending to be in a different country to watch different TV programmes, or for torrenting. VPNs are also good for protecting yourself when working in a coffee shop. For our purposes, the privacy value is in avoiding logging by your Internet Service Provider.

There are many confusing recommendations for particular VPNs online. So-called "discounts" are equally confusing. I'm probably just as confused as you, so the best recommendation I can give you is to do your own research.

## Password manager

Finally -- for now -- you should be using a different password for every site you log in to. That is far too hard, so most people use one password everywhere. Even if it's a great, secure password, you only need one website to have a data breach. Suddenly your "great" password is a "terrible" password.

The solution is a password manager, such as [LastPass](https://www.lastpass.com/) (there's a free version that's good enough for most people). This is software that creates a different, long password for every site, then remembers it for you and fills it in when you visit each website. You still need to remember one "master" password, to unlock the password manager itself. (An ideal "master" password is [five or more unconnected words](https://xkcd.com/936/).

v2019051608
