---
title: "Beyond GPS: The Hidden Ways Your Phone Tracks You"
date: 2026-08-24
# weight: 1
# aliases: ["/first"]
tags: ["privacy", "tracking"]
author: "MindDump009"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "How carriers, governments, and data brokers log your physical movements without your knowledge."
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
    image: "/img/location_tracking.jpg" # image path/url
    alt: "location tracking" # alt text
    caption: "your location is being logged" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

In order to protect our privacy online, we use services like an ad blocker, switch to privacy-focused browsers, use more focused apps, degoogle, install custom ROMs, etc. But how many of the users know that there is a serious privacy threat always following us, leaking identifiable data to data brokers and advertisers? A threat that an operating system, its settings, system/user apps, DNS, VPN, or even a firewall can’t protect us from. It is called location tracking.

Daily, every app and our carrier we use collects and logs our location in various ways without people’s attention, as this process is invisible and won’t affect device battery life or speed that much. Turning off the location or enabling airplane mode doesn’t even stop this location data collection on modern devices.

Let’s take a detailed look at location tracking and how it affects users privacy. There are several ways you can track your phone and its physical location using towers and the signal it emits. This always happens even if your device is in a privacy lockdown state.

## 1. Mobile Signal Tracking via Towers

Nowadays there are too many towers installed in our living and nearby areas by various cellular network providers. More than a perfect signal strength, quality network, or improved speed, they have various reasons related to data collection and surveillance behind this move. A single simcard with a registered network can cause serious privacy leaks to your individual life.

By these cell towers, providers can calculate where a particular subscriber’s phone is located when your phone is in a ‘power on’ state and your SIM card is registered with the network. They make it possible by using various methods, which are very accurate at their best.

### Cellular Positioning Methods

#### Cell-ID

Your phone is always looking at which cell tower it’s currently connected to to keep an ongoing call connected, send and receive messages, and make mobile data usable if it has a SIM card registered on a network.

It’s the fastest, easiest, and lower-battery-consuming way to get the position of your device without using GPS.

#### Trilateration

The network measures how fast a signal changes/switches/bounces between the phone and nearby towers to calculate the distance from each tower. By doing this they can keep the signal stable outdoors as it is indoors.

This saves phone battery when you are outdoors, as booting up a full GPS satellite chip may cause faster battery drain.

#### Angle of arrival

Nowadays cellular towers have multiple antennas pointing in different directions that measure the exact angle the subscriber’s phone signal comes from. Instead of curved circles, the tower draws straight lines crossing two lines, which mark down you fast.

Mainly used to manage a crowded 5G network. By knowing the correct angle, towers can aim laser-focused radio beams directly at the subscriber’s phone instead of sending signals in all directions. This boosts your internet speed.

#### Signal race timing

When your phone goes out of signal, it begs for at least one signal point. Nearby signal towers detect this need of signal requested by a nearby device. The closest tower hears the phone slightly before the others. With these tiny time gaps, they measure the location of the device currently in.

Mainly used to provide immediate help or assistance in emergency situations like when the person is in a no-signal area or in the middle of a forest area where satellite signals can’t reach.

#### Radio pattern matching

By driving through street mapping, they figure out how the signal bounces and signal strength is in every block. By measuring this, they will build a fingerprint for every neighborhood.

In areas with huge concrete buildings, standard math formulas to locate your phone won’t work. So your phone simply matches its live signal against that fingerprint they already created. It also allows services like Google Maps or Apple Maps to guide you through underground tunnels, concrete parking garages, or shopping malls where satellite signals won’t be able to properly reach.

#### Speed limit bumping

Cell towers constantly calculate signal delay to prevent clashes between multiple subscribers data on the same networks. As an automatic process, the network always calculates how many miles away the subscriber’s phone is from the nearest tower.

This prevents network traffic jams between different subscribers data and keeps many devices on the same tower sending and receiving data without clashing into each other’s transmission.

#### Assisted GPS

Instead of waiting a minute for your phone to search for an available satellite, a nearby cell tower sends an instant signal to your phone about where the satellite is actually now. So without much effort the phone can connect to the nearby satellite.

Used for providing instant location for delivery apps, maps, or riding apps. Then you will be able to get instant service as soon as the app opens instead of being stuck on a loading screen for minutes.

### Accuracy of Detection

The accuracy of detection can vary based upon several factors, like

* no. of towers installed
* The area the subscriber lives in
* Climate conditions.
* Number of nearby cell towers.
* The technology used by the subscriber (4G, 5G, etc.) has a SIM card inserted and registered with the cell network.
* State of mobile phone (whether powered on/off, in airplane mode, using wifi, etc.)

All the above-mentioned cellular positioning methods sound like they are used for a good purpose and make everyone’s life easier. Yes. But you didn’t see the behind scenes yet. Aside from all these good working strategies, all of our connectivity details and location data are aggressively logged and kept for years according to government needs.

Government? Yes. You heard it right. Governments have access to all this data. Because only cellular providers can do this much advanced and aggressive tracking of user location. Nowadays everyone owns a phone, and a phone without a SIM card is rare. So the government forces these operators to share a detailed log about all of them with authorities and law enforcement to monitor all users and track down lawbreaking individuals.

### Tower dump

Tower dump is a technique used by law enforcement. By this, police get a complete, detailed list of mobile phones that are actually in use and connected to a cell tower during a specific time-frame. Just imagine police asking for the cell tower logbook about guests.

This data is not only shared with the government but also with **data brokers** in order to get more money. Data brokers and advertisers pay too much for detailed and identifiable user data. The government also won’t prevent this from happening. Location data is not like other data. It’s very deeply linked with a subscriber’s current location, their past travels, who they most interact with, who they talk with more, etc… So all this data is highly valuable when it comes to certain dating apps, matrimony, insurance agencies, financiers, etc.

At the same time, **multiple carriers also share certain data in-between them**. This data is less aggressive than what they actually collected but still can be used to track an individual device. This tracking does not force carriers to turn over user data but uses the available location data on a commercial basis.

### What type of prevention method won’t work?

* Turning off GPS / Location, as this only prevents third-party apps from using and detecting user location.
* A VPN is used to encrypt your tunnel. It has no control over your physical cell tower-related tracking or device fingerprinting. But it still provides a strong protection against IP-based Geo-location tracking from websites and apps.
* Even if airplane mode is on, modern phones still keep Bluetooth, Wi-Fi, etc., turned on. Also, you can’t always use airplane mode, as it prevents calls and messages.
* Encrypted messaging apps hide your messages and transmission details that happen inside the app. But details like you used the app, how often, from, etc., are visible.

### What type of prevention method will work?

* Leaving your phone at home if you don’t need it when going outside.
* Power off the phone completely.
* Remove the SIM or disable e-SIM.

### What you can’t control

* You cannot opt out of network logging by towers.
* Even if your phone is burned, there is still a phone in another hand, also public wifi, CCTV in every street corner, etc…
* You are with your tech-savvy friend who has multiple phones in his hand, so these devices are enough to track you down.
* Using a normal keypad phone also won’t save you as long as it has a SIM card, uses 5G or 4G, and its power on always.

## 2. Cell Site Simulator

Normally the phone connects to a cell tower that gives the strongest signal to give you the best connection. A cell site simulator (also known as a **fake tower** or **Stingrays**) takes advantage of this by acting like a cell tower. It has the ability to create signals that are much more powerful than real towers can create. When your phone sees a stronger signal and it doesn't have the ability to distinguish between these stingrays and real towers, it automatically disconnects the connection to the real tower and immediately switches to this fake tower signal.

These devices are portable. It is effectively used by many governments to,

* Catch particular user mobile phones (criminals, suspected ones, etc.)
* Detect mobile users physical presence.
* Spy over users communication.

### Silent Paging

Law enforcement or operators don’t have to wait until you make a call to find you, like we saw in movies. They can send a hidden, invisible text message (group of binary) straight to your phone. You won’t hear your incoming message notification, you won't see a notification, or you won't find a new message in your inbox. But your phone’s background software receives it and automatically sends a silent reply back to signal towers. That automatic reply reveals your exact location even without your knowledge.

### IMSI Number

The IMSI number stands for **International Mobile Subscriber Identity Number**. It is a unique 15-digit code embedded permanently inside your SIM card. It is unique to every SIM card ever created.

#### IMSI catcher

An IMSI catcher is a fake portable cell tower used to capture that identity and track the device. This IMSI catcher also targets a device based upon other properties, like

### TMSI Number

TMSI stands for **Temporary Mobile Subscriber Identity**. It is a temporary, random ID assigned by networks to protect subscribers privacy.

IMSI catchers can collect local area connection logs, correlate active TMSIs, and force devices to reveal their true underlying IMSI.

### MAC Address

The MAC address is a unique 12-digit code assigned to every network interface card built into the phone. While an IMSI number tracks your SIM card on cell networks, a MAC address helps nearby local wireless networks to identify the phone.

These IMSI catchers needed to be taken to a particular area to monitor or find devices with a SIM card at that location. Anyway, this type of IMSI traffic interception by law enforcement requires a warrant to intercept the traffic and get the data of cellular network subscribers.

### What type of prevention method won’t work?

* Apps claiming to detect IMSI catchers from the Play Store.
* VPNs encrypt your network tunnel but cannot prevent a fake tower from reading your device IMEI number and logging the network.
* Turning off location services only works on third-party apps ability to detect location.
* Standard SMS and regular calls are unencrypted and easier to collect by fake towers.

### What type of prevention method will work?

* Disable 2G protocols, as IMSI catchers often force phones to use the legacy 2G networks. This type of attack is also called a downgrade attack. This is dangerous because 2G does not verify tower identity.
* End-to-encrypted apps ensure operators only see unreadable data about your communications and transmission happening inside the app.
* 5G Standalone Mode encrypts the user identity into a SUCI (Subscription Concealed Identifier) to stop IMSI catchers. But downgrade attacks forcing phones to fallback into 2G/3G networks can still bypass this unless you have disabled 2G in phone settings.

> Let me explain.

#### SUPI vs SUCI

On older networks (2G, 3G, and 4G), your phone sends its real, permanent cellular ID (called SUPI in 5G and IMSI in 4G) out into the open air without any encryption when connecting to a cell tower. Anyone with a receiver can get the signals and connect to it. 5G Standalone mode fixes this by using encryption to scramble that ID into a temporary, hidden code called SUCI. It changes constantly, so anyone who tries to intercept the network can’t get your real identity.

#### Jamming & Downgrades

5G encryption is strong, but fake towers use a cheap trick called radio jamming. The fake tower broadcasts radio noise to block or mess up the 5G signal. When your phone loses the 5G connection, it automatically falls back to older, weaker networks like 2G to keep you connected. When the connection is over 2G protocol, it broadcasts your unencrypted ID into the open air again, which causes it to completely bypass 5G protocol encryption.

### What you can’t control

When a cell tower asks for a phone to identify itself, the phone must broadcast its credentials to maintain the connectivity.

When an IMSI catcher operates in a neighborhood, it forcefully disconnects nearby devices from legitimate towers, which leads to dropped calls or disconnected data service.

When 5G or LTE signals cause interruption, the phone auto-fallbacks to older insecure protocols. IMSI catchers take advantage of this.

### Wifi and Bluetooth Tracking

We can see modern smartphones and their features have evolved a lot. Previously we used airplane mode to put our phone in a disabled/sleep state, as it prevented all connections from establishing from our phone and disabled Bluetooth, Wi-Fi, and location services automatically. But nowadays, when we turn on airplane mode, most services like Bluetooth, Wi-Fi, and location stay on. May would think, This is a new feature. This is not a feature but an advanced tracking mechanism developed for more in-depth and uninterrupted tracking via invisible signals so it won’t gain any user attention at all.

Modern smartphones have other radio transmitters in addition to the mobile network interface. They also have wifi and Bluetooth support. The signals transmitted use less power than a mobile signal uses, and they can only be received within a short range, even though someone using a sophisticated antenna could detect these signals from long distances too.

When wifi is enabled, your smartphone constantly broadcasts probe requests searching for available networks. These signals include your device’s **unique MAC address**, allowing nearby receivers to log your presence. Bluetooth operates on a similar mechanism, broadcasting short-range signals to detect paired devices.

The problem is that these unique hardware identifiers allow third parties to passively map your movements across physical locations.

The good thing is that on modern Android and Apple devices, the **MAC address is randomized by default**. This makes the tracking using wifi and Bluetooth much harder. Many phones still share a stable MAC address with connected networks, so this allows network operators to recognize and log your device whenever you return.

### What type of prevention method won’t work?

* Toggling the quick settings only disconnects currently connected networks while keeping the underlying process alive.
* Even with airplane mode on, modern phones keep Bluetooth, Wi-Fi, and location turned on.
* Using a VPN is only about network encryption; tracking via network signals and MAC address sharing still happens.
* Turning off location services doesn’t prevent tracking via network signals.

### What type of prevention method will work?

* Disabling the wifi and Bluetooth scanning systemwide will work, as it turns off the entire process.
* MAC address randomization
> (which is turned on by default on modern devices)
* Turning off wifi and Bluetooth completely inside system settings will work.

### What you can’t control

* Passing nearby another person’s device that has turned on wifi and Bluetooth scanning on their device.
> (it’s turned on by default on most phones)
* MAC randomization won’t protect you on networks that you already connected to. When you connect to a public or private wifi, they register your IP address, connection time, and browsing traffic instantly.
* Some networks need you to disable MAC randomization to get connected.

## 3. Location leaks from apps and web browsing.

GPS provides a way for the phone to detect its own location. This is implemented on Android and Apple devices with an option called ‘Location Services.’ Delivery apps, riding apps, bus/train booking apps, etc., constantly ask for this permission to detect your location and provide the service to you.

Most of these apps you share your location information with send that data to a server over the network. Then this data is shared with hundreds of databrokers it partnered with. This is a good chance for the app and data brokers to track you. Maybe the app developer himself doesn’t mean to collect any data like this, but it’s all about the terms and conditions of services you are using. Also, this will end up in revealing your location information to the government and data breaches.

Location data is not only about the present location of your device or you. It’s more about the historical activities, beliefs, participation in events, personal relationships, etc.

> For example,

Various dating apps used location data to suggest partners or detect who certain users are mostly interested in, in which place they spend most of their time, who attended a particular meeting, who participated in protests against governments, identify journalists, etc.

Many past incidents have revealed location data collected by various popular apps are purchased by governments and law enforcement to track down individuals. This included both real-time and historical data.

### Real-time bidding

Most of you think app developers directly collect and sell your location, right? But mostly, the real leak comes from in-app advertisements. When you open an app with ads, the ad network runs a split-second auction behind the scenes called Real-Time Bidding (RTB) to decide which ad to show you.

### Bidstream

To get buyers to offer more money for higher ad space, the app automatically broadcasts a data packet called a BidStream to thousands of advertising companies in milliseconds. This packet includes your GPS location, IP address, and your phone’s Advertising ID (MAID). Even if an ad company loses the auction and doesn’t show you an ad, they still keep that BidStream data, which allows data brokers to build a massive, real-time data profiling of everywhere you go.

### What type of prevention method won’t work?

* Togglings that quick-access GPS button stop direct system calls, but some malicious or aggressive apps like social media, games, etc. will still get access to it.
* Trusting in the in-app privacy policy, like data is anonymized, data is never shared with anyone, etc. Location data is never anonymized, and it is shared with many data brokers.
* In-app consent saying what data to share and what not to share is just a way to make users believe they collect minimal data. Behind the scenes, nothing is changed.
* Force-closing apps stops its main code, while background services are still active.
* **Free VPN's*** don’t protect but harvest user data for money.

### What type of prevention method will work?

* Changing the location access level from **alway.** to **never** or **while using**.
* Turning on approximate location will give apps a broad region instead of an exact location.
> (still identifiable and does not equal spoofing)
* Removing exif data (metadata) before sharing images helps remove embedded location details in photos taken using a mobile camera.
* A DNS can prevent the collected data transmission if the data is sent to a domain name. 
> (If it’s direct IP transmission, then DNS won’t help)
* Disabling network access with local firewall apps might limit the transmission of location data that happened.
> (But remember, many of these apps strictly require network access to work)
* Ditch proprietary apps and switch to privacy-friendly FOSS alternatives.
* Use a custom ROM like GrapheneOS over stock ROM.
* With root access, users can use the location spoofing option only in supported custom ROMs.

### What you can’t control

* A malicious app injecting ad/tracker code can bypass device-level protections and still transmit location-related data. The solution is to never install unknown apps.
* Your IP address can be pointed to your real location. (A VPN can hide your IP.)
* Location data collected by 1 app will be shared with hundreds of data brokers and partners.

## 4. Behavioral Data Collection

In addition to location tracking, many apps and games harvest telemetry data to build unique user/device profiles. This includes:

*     App telemetry: 
	* installation history.
	* app launch frequency.
	* active usage statistics.
*     Device state: 
	* battery percentage.
	* charging status.
	* time zone.
	* system orientation.
*     Persistent identifiers:
	* mobile Advertising IDs (MAID).
	* unique system parameters.

All this information is shared with hundreds of data brokers and third-party companies. Even if this data looks so basic, an aggregation of this can reveal a lot of identifiable information and will be used to generate unique tracking profiles for each device.

Major advertising companies like Google, Meta, Amazon, etc., convince users to install a small bit of their tracking code inside developers apps in the name of verification, monetization, access to app stores, etc. With these small bits of tracking code, now companies are able to place advertisements inside the app.

Also, the sharing of location and behavioral data did not only happen one time; it was re-shared across many advertisers, service providers, and data brokers. An average mobile user has no idea about this at all, which is disturbing.

> At the time you are reading this blog, there are chances that you also have a detailed profile on any data broker’s database.

## 5. Mobile Advertising Identifier (MAID)

With MAID, this collected behavior data becomes actually useful to the data brokers. MAID is a random unique number that is used to identify a single device. Advertisers and data brokers pool together the data they collected from different apps using MAID. Then they build profiles based on the MAID ID generated for each device.

On Android, every preinstalled, third-party app has access to MAID by default.

### What type of prevention method won’t work?

* Resetting advertising ID.
* Incognito / private browsing mode.
* Airplane mode.
* VPNs.

### What type of prevention method will work?

* Custom ROMs like LineageOS, GrapheneOS, etc., which are degoogled.
* Opting out of app tracking. (Mostly works on iOS, not on Android)
* Deleting the advertising ID in the system settings will wipe the main ad code.
* Using privacy-focused browsers.
* Revoking app permission or using a local firewall.

### What you can’t control

* The device fingerprint, combined by various factors like battery level, IMEI number, apps installed, etc., is unchangeable. But it can be minimized or restricted by the installation of a more privacy-friendly OS and switching to FOSS apps. 
* If you are installed apps owned by major advertising company on your phone, then you can’t control how these apps collect and use your data. For example,

	* Meta owned instagram, facebook, and whatsApp.
	* Google owned apps and it's proprietary play services and various apps.
	* Amazon owned apps like amazon shopping, amazon app store, etc.


* After the data leave your device, you have no control over it; it is shared by and profiled by so many data-brokers, advertising and non-advertising companies, government, etc.

## 6. Conclusion

Our location data is being leaked from phones in many visible and invisible ways that we are not even familiar with at all. From governments to databrokers, everyone needs our location data. Because it bridges the digital world identity with our real-world identity.

Daily, these collected location data have been effectively used for

### Predictive behavior profiling

Your time-spending habits reveal socioeconomic status, religion, medical condition, relationship status, and more.

### Hyper-targeted monetization

A data broker will charge more from advertisers if they are able to prove an ad makes the individual walk into a specific store.

### Risk modeling and real-time tracking

Widely used by insurance companies and agencies to sell products to specific users. Using the location data, they can measure financial risks, property risks, preferred insurance rates, determine to whom we planned to vote for and manipulate our decisions, etc…

### Unreliable but powerful solutions

Not everyone has to follow these many strict moves in their life. The choice is completely up to the individual and based upon their threat model. These are the 3 choices decisions I took to eliminate most of the surveillance and tracking from my life.

#### Free and open-source apps

Switching from proprietary apps to free and open-source apps can drastically change the amount of data collected from your device. These apps are designed to be lightweight and distributed under a free license that anyone can use or modify for free. These apps are primarily published on trusted app stores like **f-droid**. This strategy doesn't require a custom rom installation, rooting or degoogling. Just install and enjoy.

#### Degoogling

This helps to strip down all Google-related services from android phone and still use the phone with possible comfort and usability. There are many ways available to achieve this.

* Using **adb** via laptop to uninstall bloatwares or alternatively anybody can install the software called **universal android debloater** on their linux or windows systems.
* Using an android app called **canta** within android with the power of **shizuku** to debloat android.
* unlock the bootloader to install a more lightweight and faster **custom ROM** like lineageOS, grapheneOS, calyOS, etc.
> This will also increase the life-span of your android device.

#### Custom ROM

An entire switch from stock ROM to a more free and lightweight OS can be relaxing and satisfying. When compared to stock ROM, custom ROMs are more privacy-friendly and well maintained. Gives more life span to the device.

##### Requirements

* A phone with unlocked bootloader.
* Compatible custom ROM image.
* Recovery.
* A pc or laptop with adb and fastboot tools installed.
* Internet connection.

---

Hope you guys found my blog post article useful.

Thank you for reading.