---
title: "DNS: The Phonebook of the Internet"
date: 2026-08-27
# weight: 1
# aliases: ["/first"]
tags: ["security", "privacy"]
author: "MindDump009"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "Explaining how DNS works and why its important to choose a secure DNS provider!"
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
    image: "/img/domain_name_system.jpg" # image path/url
    alt: "DNS" # alt text
    caption: "DNS" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

In the past everyone used direct IP address to visit websites over the internet. Nowadays, people remember simple domain names. Instead of remembering and typing a group of complex numbers, users are now able to directly type the domain name (duckduckgo.com, privacyguides.org, startpage.com, etc.) on the URL bar to visit and browse the website they want.

Ever thought, what triggered this change? What allows us to comfortably remember domain names instead of complex IP addresses of millions of website? This service is called DNS.

## DNS

DNS stands for Domain Name System. DNS is the phone-book of internet. Humans access information online via domain names like duckduckgo.com, privacyguides.org, etc. while web browsers communicate and interact with website via IP addresses. DNS stands as a bridge between them by translating domain names into IP addresses. 

By the implementation of DNS, users no longer have to remember IP addresses of billions of websites. This also makes retrieving information much easier and faster.

### Domain names

We can describe a Domain Name as a label for a website.

Naturally, computers can't understand words, instead they use a combination of numbers differentiated with (.) dots called IP address (142.250.190.47) to find websites on the internet.

A domain name replaces these IP addresses with a memorable name. When a user types the domain name like duckduckgo.com into a browser URL bar, DNS looks up the number inside its massive public records of IP addresses to find the IP corresponding to that domain name and helps you to connect to it.

### IP address

IP address stands for Internet Protocol Address. IP address is a unique string of numbers assigned to every device connected to the internet. It acts as a digital identity given to every internet user to uniquely identify them.

#### Purpose

IP address lets computers, servers, and other devices related to internet distinguish themselves from millions of other devices online.

It routes the internet traffic. When opening a website, the request uses your IP address to tell the server where to send back the loaded website so you can access them without issues.

There are two types of IP addresses available today.

#### IPV4

The old addressing format. This written as four sets of numbers separated by dots.

Looks like, 142.250.190.23

The internet actually ran out of these addressing formats, and switched to a new format.

#### IPV6

The modern standard of IP address formatting. Longer strings of numbers and letters separated using colons.

Looks like, 2607:f8b0:4005:802::200e.

It provides virtually unlimited number of IP address combinations.

Without IP addresses, a device cannot communicate over a network.

### URLs

URL stands for Uniform Resource Locator. It is the web address you type into the URL box of the browser to reach a specific website.

It starts with **HTTPS (Hyper Text Transfer Protocol Secure)** known as **Protocol** and continues with **WWW (World Wide Web)** and the domain name.

Looks like, https://www.duckduckgo.com

#### Properties of a URL

* **Protocol**: A set of rules the browser uses to talk to the server. It tells the browser, how to fetch data securely.
* **Domain and Subdomain**: Name of the server, where website is hosted. (This is what a DNS translates to IP address).
* **Path**: The specific page or path a user wants to access on that server that stored inside the specific website you are in. For example, https://www.duckduckgo.com/about
* **Parameters**: Extra details passed to a page, often used for tracking source, search, or filter content like safe search.

### Domain extension

A **TLD (Top Level Domain)** is the ending of a domain name right after the last dot.

For example,

* duckduckgo.**com**
* nextdns.**io**
* privacyguides.**org**

#### TLD categories

* **gTLDs (Generic Top Level Domains)**: These are general purpose domain name extensions used by anyone globally.
	* **.com**
	* **.org**
	* **.net**
	
* **ccTLDs (Country Code Top Level Domains)**: These are two letter domain extensions reserved specifically for countries or territories.
	* **.ca**
	* **.de**
	* **.cn**
	
* **sTLDs (Sponsored Top Level Domains)**: Restricted extensions managed by specific agencies or strict authorities.
	* **.gov**
	* **.edu**

## Working of DNS

The **DNS lookup** happens in the split second between typing a URL and the page loading. In this time DNS completes the conversion process. There are 4 main DNS servers involved in the lookup.

* **Stub resolver**: The browser or ISP server handles the request.
* **Root server**: Points the request to right area based on the domain extension (.org, io, .com, etc.).
* **TLD server**: Directs the request to specific domain's authority.
* **Authoritative name server**: Holds the exact IP address and delivers it back to the browser.

### DNS caching and speed

In reality, your browser doesn't have to perform these steps always. Because there is a DNS caching functionality inside every modern browsers we use.

* **Browser DNS caching**: The browser remembers recent sites you visited on its local memory. So there is no need to perform DNS Lookup every time you search for the same website which significantly increases browsing speed.
* **TTL**: TTL stands for **Time To Live**. It means how long a DNS record is allowed to sit in memory until browser forcing a fresh lookup.

### Local memory and caching

Actually local memory is a **temporary storage** located on the physical device you are using. When browser stores a DNS entry locally, it holds onto that IP address mapping directly on your local machine without connecting to any external server.

**Local DNS caching**

Local caching happens across three layers of the local machine you using before reaching the network.

* **Browser cache**: Modern browsers have their own internal DNS cache in memory to resolve the sites recently visited faster.
* **OS cache**: If the browser doesn't find the entry in its own cache, it asks the local OS resolver to store the cache in its system memory temporarily.
* **Router cache**: If the OS hasn't cached it, then the request goes directly to WiFi router, which often keeps recent DNS lookup caches inside its cache management functionality for all devices connected to it.

If the DNS lookup fails to resolve the domain name from these three local cache layers, it directly establish a connection to the server over internet.

## DNS Privacy & Security Risks

Standard unencrypted DNS (over port 53) poses several security and privacy risks to its users. Some of them are,

* **ISP snooping**: Plain DNS queries are sent as readable clear text. Your **Internet Service Provider** can log everything, even if the website uses HTTPS. *(If the site is encrypted, then the site contents are hidden from ISP, but they still know you visited this domain along with its metadata.)* 
* **DNS leaks**: When using a VPN, unencrypted queries can bypass secure tunnels and expose browsing data to local resolvers. *(All modern VPN services like ProtonVPN, MullvadVPN, IVPN, etc. have its own encrypted DNS turned on along with VPN. So it doesn't matter even if you are using a secure custom DNS, if you are using these reputed VPN providers. Am not sure about what the case is when it comes to VPNs you downloaded for free from play store, or others like NordVPN, Surfshark, Private Internet Access, etc.)*
* **DNS hijack and spoofing**: Attackers can easily intercept and log your browsing activity if you use an unencrypted DNS server. They can even redirect you to a malicious IP address.

## Encrypted DNS solutions

There are several well tested and recommended methods to secure your DNS queries for free. These include,

* **DOH (DNS Over HTTPS)**: This encrypt DNS queries using the standard port 443. So it blends with normal web traffic, which makes ISPs cannot block or monitor specific domain request.
* **DOT (DNS Over TLS)**: Encrypt DNS queries using standard port 853, securing queries system level. However, DOT runs on its own dedicated port 853. So ISP can easily identify that you are using an encrypted DNS.
* **Public resolvers**: There are many free privacy focused public resolvers available to consider when the aim is encryption, faster resolution, customization and privacy. These are trusted, non-logging and with advanced features.

---

> **Our ISPs provide DNS by default which covers almost all websites IP available on the internet. But the main issue is that, it is unencrypted. Unencrypted for decades, and they never even bothered to encrypt it and they really don't want to. Also we are in a danger of direct government influence. If government ordered to block any website, ISP must follow it. So with a plain text DNS resolver, we are extremely censored. Also in the past, many noticed that ISP intentionally throttling downloads, streaming websites to save bandwidth for other users, even if we paid for the network we use.**

---

**Recommended public resolvers**

	* Cloudflare
	* Quad9
	* NextDNS
	* ControlD
	* Adguard DNS
	* Hagezi DNS
	* uBlock DNS

### Common myths

* Encrypted DNS doesn't unblock ISP blocked websites or domains.
* Even if connection is now encrypted, ISP can see the domain names we visit without a VPN.
* Encrypted DNS doesn't bypass ISP throttling.
* Encrypted DNS doesn't hide the data rate you consumed, you online presence, protocol you used, etc.
	
## Conclusion

Encrypted DNS resolvers are very essential in our life as our every communication over the internet to domain names happens over a DNS query. As we said, if your queries are unencrypted, it is much easier to intercept those request and log it by ISP or any hijckers.

---

Hope you found this article  useful.

Thank you for reading.

