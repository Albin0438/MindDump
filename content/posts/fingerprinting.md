---
title: "Fingerprinting: The Hidden Trap on the Modern Web"
date: 2026-08-18
# weight: 1
# aliases: ["/first"]
tags: ["fingerprinting", "privacy"]
author: "MindDump009"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "Explained various fingerprinting methods used in the modern web and what to do about it."
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
    image: "/img/fingerprinting.jpg" # image path/url
    alt: "fingerprinting" # alt text
    caption: "fingerprinting on web" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

Nowadays online privacy is almost dead. Even in the comfort and dopamine loop we get from social media and the web, we also started to forget about the importance of privacy on the web. A single website owner to big corporations, including governments, has most of our browsing data, more than they need to protect us. Our every move is cleverly traced and kept for years without any security at all.

One of the most effective methods used to identify a person and the device he uses is fingerprinting. "Fingerprinting" isn't just a word that indicates something, but it is the pipe they use to transmit or extract all our data (the device we use, operating system, installed fonts, etc.) via every single website we use. For monetization and earning, every single website owner injects tracking code into their websites without even knowing the full story.

## What is fingerprinting?

It is a method used to identify a particular browser, extension, hardware, or user by collecting and combining various data like

- Browser version
- Extension installed
- timezone and system-level language.
- Installed audio and video codecs
- Installed fonts.
- Browser settings tweaks.
- device resolution and size.
- Browser window size
- Using an operating system

and much more data.

They collect it and combine it to identify users at different browsing sessions or even for cross-browser tracking.

### Is this much data directly provided to every website we visit by default?

Yes, of course. All this data is automatically collected and stored on the server when we visit websites with our most used browsers (Chrome, Edge, Firefox, etc.). It’s not cookies; it’s creepier and permanent compared to it.

But some other privacy-focused browsers (Mullvad, LibreWolf, Tor Browser, Brave Origin, etc.) prevent most of this data from getting leaked to websites we visit. Or they just spoof the values with a fake one, so the collected data becomes useless.

## JavaScript: The Real Danger

JavaScript is a scripting language we use to write scripts. It provides added functionality to browsers and websites. What else can a normal scripting language do other than build some scripts. Right?

Not at all. JavaScript is the tool all these websites use to harvest this much information from our devices. JavaScript is very useful, and at the same time it exposes a lot more than we can imagine about our browser and device.

> JavaScript depends on web APIs to run invisible background tasks for getting system details. This includes hardware info, RAM, screen size, timezone, etc.

### Types of fingerprinting using JavaScript.

Imagine JavaScript is giving a tiny task to your computer. By analysing the way user's system process the task, JavaScript measures specific hardware on the system that is used to complete the task.

Look at some fingerprinting methods effectively usable and continuously used with the help of JavaScript.

### 1. Canvas fingerprinting (2D Graphics)

- Canvas is an HTML5 element used to draw 2D graphics and text directly on a webpage.

**How does fingerprinting work?**

- JavaScript asks the browser to draw a 2D image with specific colors and shadows.

- According to the operating system, graphics driver, and graphics card, the way the system processes anti-aliasing is a bit different.

> Anti-aliasing is a method used to smooth out the edges.

- The script notices these differences and renders those pixels into a text hash, creating a unique code.

### 2. WebGL fingerprinting (3D Graphics)

- WebGL is a browser API that allows sites to render 3D graphics.

**How does fingerprinting work?**

- WebGL just directly asks the user's system for its GPU's manufacturer and model name.

- It also forces the GPU to render hidden 3D objects. By the time the system completes the task, the script detects the tiny difference between GPU renderings and stores it.

### 3. WebGPU fingerprinting

- WebGPU is an improved version of WebGL.

- It does exactly what WebGPU does but with more added capabilities like low CPU overhead, multi-threading, etc.

**How does fingerprinting work?**

- WebGPU sits closer to actual hardware, which means it transmits even more accurate data than WebGL does.

- It detects and stores structured information about adapter features, exact texture formats, WGSL language support, etc.

- This fingerprinting method is much faster and extremely accurate.

### 4. Audio fingerprinting

- The web audio API allows browsers to generate, process, and play audio directly in the browser.

**How does fingerprinting work?**

- A script sends a silent sound wave through standard audio tools like an oscillator and dynamic compressor to make the system actually process the audio.

- Sound waves are converted into long decimal numbers. To handle it, hardware needs to round it and store it somewhere. This rounding process depends on the combination of hardware and software the system has.

- The output has a difference of microscopic fractions at the end compared to audio processed by someone else's computer.

- The web audio API script notices and records it.

### 5. Font fingerprinting

- A technique used to detect all installed fonts on the system.

**How does fingerprinting work?**

- A script writes hidden text snippets on a page using non-existent fonts so it falls back to the default font size.

- Then it swaps that font for hundreds of well-known and widely used fonts. (helvetica, sans-serif, verdana, etc...)

- If the text size changes when measuring the pixel width, then the script understands the font is installed on your system and records it.

### 6. Other common fingerprinting methods

JavaScript uses every possible way to collect much data from the website other than graphics and audio.

**Hardware specs**

- Collects the CPU's exact core count and system RAM

**Screen & display parameters**

- Collects screen width, height, available workspaces, color depth, pixel density, etc.

**TLS/Network handshake**

- Collects the order and types of encryption cipher the connected HTTPS network support

> This is completely doable without Javascript too.

**Time zone**

- Collects system preferences regarding language, timezone, keyboard layouts, etc.

### From Fingerprints to Individual Data Profiles

All this fingerprinting is done using a single scripting language, JavaScript, by a single website.

With all these collected metrics, the site now knows almost everything about the visitor's device and browser he used. So it combines all the collected information into a single profile to create a detailed, unique identity about the user. Then whenever this user revisits, maybe from a different browser or using a VPN, the browser scans all data profiles it has and tries to match currently detected information to existing profile data to identify the user uniquely. This is called "fingerprinting."

> The interesting fact about fingerprints is that they can't be deleted or tweaked by the user like clearing a cookie. Also, even a VPN can't protect from fingerprinting.

## Why prevent fingerprinting?

- Cookies can be cleared; the fingerprint is permanent.

- Your privacy is more important than you think. Seriously...

- A VPN can't protect you if they have a unique fingerprinting record on you.

- Effectively used for cross-browser session tracking and identification.

- Your real-life identity doesn't have to be linked to your normal browsing data.

> They are building unique profiles about you, and they never expire. These are shared across many business partners, and there is nothing to wonder about when you see an ad while browsing about what you just talked about. Also, this data is used in more disturbing ways than someone can imagine. They know in the modern day, data is the valuable thing even though you really don't know how valuable online privacy is.

## What are the solutions?

> Please avoid MV3 browsers, as the techniques/extensions I explain below have very little effect on these browsers.

### Ublock Origin

- Use an adblocker?. No. Ublock is not an adblocker. It's a content blocker that does more than just blocking ads.

- It stops the fingerprinting scripts from executing in the first place.

### No Script.

- Gives much more control over scripts run on a website.

- You can decide to allow a website to run scripts at all, which scripts to allow, and which ones to keep off for every website you visit.

> It is very inconvenient to use when it comes to normies. But it's the user's problem and has nothing to do with this extension.

### Privacy-hardened browsers.

- Many community-maintained browsers come out of the box with tweaks for privacy, including fingerprinting protection.

**Recommended Browsers**

- Tor Browser (the king)
- Librewolf
- Mullvad
- Brave Origin
> Suggesting Brave Browser is controversial in privacy communities due to its shady practices in the past, but at the same time, it prevents fingerprinting effectively out of the box.

## What makes fingerprinting more accurate?

- Installing too many custom fonts.
- Using common browsers like Chromium, Chrome, Edge, Vivaldi, etc.
- Installing too many extensions.
- trusting random fingerprint spoofing extensions or scripts.
- Browser settings tweaks.
- window resizing.
- Hardware setup.

### Browsers you must avoid

* Google Chrome
* Microsoft Edge
* Vivaldi
* Vanilla Firefox without tweaking for fingerprint resistance.
* Standard safari

> When it comes to vanilla Firefox, it out of the box provides no protection against fingerprinting at all. But it can be tweaked for effective fingerprint resistance.

There are various user.js files available to harden Firefox.

1. [Betterfox](https://github.com/yokoffing/Betterfox)
2. [Phoenix](https://github.com/celenityy/Phoenix)
3. [Arkenfox](https://github.com/arkenfox/user.js/)

## How to test your fingerprint detection score?

These are various free tools online to check how much the browser you use exposes about you.

**[Cover Your Tracks](https://coveryourtracks.eff.org/)**

- Founded by the Electronic Frontier Foundation.
- Shows a detailed summary on what was protected and what was not.

**[Am I Unique](https://amiunique.org/)**

- Gives fingerprinting details based on your current settings and setup.

**[CreepJS](https://abrahamjuliot.github.io/creepjs/)**

- It dives deep into systems graphics drivers, WebGL, system fonts, and audio frequencies and then gives a clear output on whether your browser is capable enough to prevent fingerprinting.

<br><br>

Hope you find this article useful.

Thank you for reading.