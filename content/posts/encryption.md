---
title: "How Encryption Powers the Internet."
date: 2026-08-25
# weight: 1
# aliases: ["/first"]
tags: ["security"]
author: "MindDump009"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "Taking a deep dive into the working of encryption on the modern web."
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
    image: "/img/encryption.jpg" # image path/url
    alt: "encryption" # alt text
    caption: "encryption" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

In the modern internet most of our daily activities on the internet like browsing data, transactions, calls and messaging via encrypted messengers, dns queries, https protocol, etc. Still many of us don't really know what exactly an encryption is and how it works. Let's take a deep dive into it.

## 1. What is Encryption?

Encryption is a method of converting actual data into a unreadable scrambled format (known as ciphertext). The process is done using various mathematical operations, algorithms and complex digits. The encrypted data is locked with a instantly generated cryptographic key to prevent decryption by anyone on the internet. So only who have the matching encryption key can unlock and read the encrypted data.

The process of generating keys are done using a method called TLS Handshake.

### CA Certificates

CA Certificates are a collection of root certificates that are used to verify the authenticity of web requests and connections by various apps working over internet. For example web browsers, banking apps, messenger apps, app stores, etc.

Every connection happened on the device strictly require validation from these CA certificates. otherwise the data transmission will be interrupted.

These are created by legally trusted providers like DigiCert, Let's Encrypt, Sectigo, etc.

### TLS Handshake

TLS handshake is a method used to generate exact same cryptographic code before the encryption process. So both party can encrypt the data with a matching cryptographic code to make the data readable for user.

During this process the computer and server shares a non-secret mathematical clue across the internet. using a mathematical technique both devices independently calculates an exact same cryptographic key at the same time.

The clue is non-secret because it is a public number created by math and doesn't pose any privacy or security risk by sending over the internet.

Without this code anyone on the internet can decrypt the data using the same algorithm used and read it without sender's permission. A secret code makes sure that this won't happen.

## 2. Types of Encryption

Encryption is done using types of mathematical formula and algorithms. but specifically there are 2 types of encryption is available.

### Symmetric encryption

Symmetric encryption only uses a single secret key to scramble and unscramble actual data

In this type of encryption mechanism, both sender and receiver have the exact same key, which is a faster and efficient method to handle if there is a huge amounts of data.

**For example**, a normal lock that have exact same keys used by both members in the same house to open the door.

### Asymmetric encryption

Unlike in the symmetric, asymmetric encryption uses a pair of keys to scramble and unscramble the data. Those keys are known as **public** and **private** key.

In here, you send your public key to the other person over the internet. Using the public key other individual can send you encrypted messages that only your private key can decrypt and read.

**For example**, a person drops a letter on your personal mailbox. Here mail box is the public key. Nobody else walking near the mailbox can open or access the main box until you reach the mailbox and open it with your private key.

## 3. Why Encryption?

### Protect privacy

Encryption helps to hide the actual data. So it makes sure that the real data is secure from online threats like hackers, man-in-the-middle attacks, etc. It is much more safe to send a photo, make payments, or entering credit card number on a website using encryption than sending it over plain text.

### Prevent data altering

Encryption makes sure that data never get altered. Because the way of scrambling the actual data is based on a chosen algorithm used by who encrypted it. Using a different method to decode or rewrite the data is often ends up in useless corrupted data format.

### Verify authenticity

Encryption methods allow the browser or certain app to verify that the web server is authentic and protected. By the combination of various factors like digital signatures, CA certificates, the encryption makes sure that the user is talking to the actual bank or government service rather than a phishing/fake site created by malicious actors to steal your data. Usually known as **man-in-the-middle attack**.

#### Man-in-the-middle attack

A malicious actor intercepts the communication between two and relays it when the communicators believe they are talking directly each other without a third person's presence.

This usually happens in communication mediums that lacks encryption. For example, **standard sms**, **phone calls over ISP**, **http traffic**, **insecure public-wifi**, etc.

### Legal standards

Even government requires companies that handle sensitive information over the internet must use encryption by default. This verifies confidential government data about citizens never get leaked or spied by other country hackers, etc.

European GDPR, US HIPAA and PCI-DSS like laws are exact example for this.

### Security on cloud platforms

In modern internet most of the companies switched to work from home like mechanisms and these have a big dependency over popular cloud platforms like amazon. azure. google cloud, etc.

Encryption makes all the data transmission and storage on this cloud platforms secure and protect millions of companies private data from hackers, threats and other types of attacks.


### Physical Decice security

A lot of peoples store their private information on their phones and laptops. When carrying this on traveling pose the risk of forgetting it somewhere or get stole by someone. This will lead to a massive privacy invasion as it already have your important data decrypted.

Modern features like full disk encryption or encryption on booting will prevent the malicious actor from booting your device app. Which can be useful to protect your privacy 
within a limit.

### Network security
 
 All the services and functionality on the web transmit data over networks. In the history web used a protocol like **http** to communicate and transmit data each other. The founding of encryption leaded to a more secure and trusted protocol called **https** by default.
 
 Currently websites uses http instead of https are very rare.
 
 ## 4. Disadvantages of encryption
 
 Every inventions ever created has disadvantages. Same goes for encryption too. Let's look at what are the disadvantages of encryption.
 
 ### Data loss
 
 After encrypting, if you lost your private encryption key, recovery password, or master key data remains scrambled forever. There is no forgot or restore button for powerful encryption algorithms.
 
 So it is much more important to keep the master key, private key or even recovery key in a separate space like a password manager to always ensure you have access to the encrypted data.
 
 ### Performance
 
 Scrambling and unscrambling is not a very lightweight process on CPU. It does need its own processing power. While smaller files only take a small amount of CPU and power, larger data can take up to a significant amount of power CPU power.
 
 When it comes to encryption of operating systems on laptops, you can notice this as the bootup process can be slower.
 
 ### Key management
 
 Generation of key is faster and simple process. But storing, distributing, and backing up them securely across thousands of devices and employees is a crucial challenge for IT teams that include too much complexity.
 
 Also a compromise of private key can collapse all the security provided by using that key.
 
 ### Maintenance cost
 
 For many companies like maintaining a online messaging app, social media, blogging platform, banking services,etc. maintaining a setting up and maintaining a military-grade encryption requires special hardware, digital certificates, dedicated software for managing keys and personally trained employees which can end up in a huge expensive setup.
 
 ### Misuse by bad actors
 
 Cybercriminals and malicious actors use encrypted channels and HTTPS connections to deliver malware or other types of threats that can steal user data. Because this data is encrypted, it's often hard for the security software to detect and block.
 
## 5. The misuse of encryption

Aside the advantages and disadvantages of encryption, it is actively misused by malicious actors.

### Ransomware

Encryption technique is actively used across computers to spread ransomware. Cybercriminals breach a user's network, access their important files and use powerful encryption algorithms to lock down their hard drives, cloud storage, and databases.

In this process, the victim's data is converted into an unreadable form of scrambled data and demands money or cryptocurrency in order to decrypt these encrypted files.

> **Note: There is no guarantee that after they get the money or cryptocurrency, the data will be back to its normal form. Also if yes then still most part of it can be corrupted.**

### Bypassing security software

Modern security software is integrated deeply into system. This software scan the system 24x7 and instantly spot any known threats. They easily detect malware signatures and unauthorized data transfers. So hackers hide their network activity inside an encrypted HTTPS tunnel. This will prevent security software from identifying those malicious data transfer in real-time.

Most cybercriminals host malware on encrypted websites as network firewalls cannot inspect the payload in transmission to flag or block it.

Once outside the corporate network, attackers encrypt databases inside the network before sending them back to their external servers known as **data exfiltration**. For security tools this looks completely normal.

### Misuse of being anonymous

**TOR** stands for The Onion Router. The Networks like **TOR** rely upon multiple layers of encryption to route the internet traffic via decentralized nodes by hiding a user's real IP address and location.

This type of protection and anonymity is very helpful for dissidents, journalists, and whistleblowers working under tight surveillance state. At the same time it is actively used by many hackers and criminals to host illegal goods, stolen credentials beyond the reach of law enforcement.

This is also a reason for increased surveillance across countries and governments attacks against anonymized networks like TOR.

### Illegal communication channels

End-to-End Encrypted messengers ensures that all communication happened inside them are tightly encrypted and secure from a third person. This also prevents telecommunication providers, platforms, governments from snooping on user's chat history and personal messages.

As usual, criminals, terrorists, and extremist groups take advantage of these platforms to plan illegal activity, conduct child sexual acts, distribution of drug, selling stolen materials, etc. So this cannot be decrypted and read by law enforcement even with a court warrant.

## 6. Recommended tools for daily use

Encrypted tools are not only limited for big corporations or governments. These are a must have tools in every individuals life. There are many tools that provide meaning to our daily activities and ensure our data is completely secure at a preferred comfort level.

Let's look what are some free encryption tools we can daily use in our lives. These tools never become inconvenient or another tool for stealing your personal data, instead it gives a more productive workflow and organized private life.

> **The recommendation is based upon security and privacy (how they handle user data).**

### Messaging apps

Unlike standard sms and phone calls, communication via a encrypted messaging app is encrypted using strong algorithms and this will prevent our telecom providers, malicious actors, governments from intercepting and snooping on our communication.

Not all messaging apps available today are encrypted and designed to protect our privacy. many of these apps collect information about the user them-self and sell to data-brokers and governments.

**Recommended Messaging apps**

* Signal messenger
* Session messenger
* SimpleX chat
* Matrix
* Threema
* Briar

**Not recommended**

* Whatsapp messenger
* Telegram Messenger and it's forks
* Facebook Messenger
* Instagram in-built chat

> **WhatsApp uses end-to-end encryption for messages but collects metadata, telegram is not end-to-end encrypted by default).**

### Password manager

You no longer have to use that **password@123** on every single site to sign-up and keep remembering it. Instead with a password manager you can generate a much secure and stronger password and store it inside it. So you only have to remember you master password from now on as all the other credentials depend upon this master password to get unlocked and used.

In modern days password managers offer much more features like,

* two-step verification
* YubiKey support
* notes and cards section
* pass-keys

> **Keep in mind that your all other login credential are now protected via a single master password. So it's your responsibility to make sure that this master password is not password@123.**

**Recommended password managers**

* KeePassXC (offline)
* Bitwarden
* Proton pass

### Two-Factor authenticators

A most effective and widely adopted method of two-factor authentication. The method this app follows adds a second layer of protection for all your online accounts.

This provides a security codes that gets expired within seconds. If you are enabled this authenticator app inside your online account security section, then every time you login it asks for that secure code appeared inside the authenticator app.

Modern authenticator apps are very convenient as most online accounts will provide a recovery method if you lose access to that authenticator, many authenticator show the upcoming security code so if one is too close to expire stage then you already know the upcoming code.

**Recommended authenticators**

* Ente auth
* Proton authenticator
* Bitwarden authenticator
* Aegis authenticator

### Cloud storage

Cloud storage platforms help you to store your files and documents on the cloud. By using this functionality you can save your local storage space while still keeping all you important files on a secure cloud.

**Recommended cloud providers**

* Nextcloud
* Proton Drive
* Filen.io
* Koofr
* Icedrive

**Not recommended**

* Google drive
* Onedrive
* Dropbox

> **Google Drive, OneDrive, and Dropbox use standard encryption for security, but they hold the decryption keys themselves. Means they are not client-side encrypted.**

> **Many people use telegram as a free cloud storage functionality but it is not recommended at all. Telegram is an unencrypted messaging platform (secret chats are only encrypted). Furthermore, if Telegram suspends your account unexpectedly, you lose access to all your files.**

### Photo storage

Like cloud storage for files, there is platforms provide functionality to store all your memories (photos) online. Because this are specifically designed for storing photos, this platforms provide in-app features to edit and modify the images.

**Recommended platforms**

* Ente photos
* Proton drive (in-built photos section)
* Stingle photos

**Not recommended**

* Google photos

### DNS providers

Unlike old days, there is no need to stick with our ISP's unencrypted DNS service. There are much better, encrypted, faster and customizable DNS servers available for free.

**Recommended providers**

* NextDNS (customizable with adblock capability)
* ControlD (free tier have pre-configured categories for multiple purposes like adblock, malware block, etc.)
* Quad9 (powerful threat blocking capability than many paid services)
* Cloudflare (while default address give no filtering but high speed experience, users still have options to use DNS with malware blocking and malware + adult content blocking depending on the address.)
* Mullvad (adblocking dns from a trusted VPn provider)
* Adguard dns

**Not recommended**

* ISP's own dns (unencrypted)
* Google dns
* CleanBrowsing
* Comodo secure dns

### E-mail service

E-mail services are still effectively use by many companies and individuals to communicate. even though it is not the best method of communication, it is still reliable for most. So using a secure and trusted service for handling emails are very important.

**Recommended providers**

* Protonmail
* Tuta
* Startmail
* Mailbox.org

**Not recommended**

* Gmail
* Outlook
* Yahoo mail
* Zoho mail

### Web browsers

More than the implementation of **HTTPS** protocol using a trusted browser for daily browsing is very essential to stay secure and protected. More than strict encryption, these browser provides added layer of privacy by certain features like,

* link upgrading to https
* ad/tracker blocking
* fingerprint protection
* faster navigation
* productive features

All browsers are not the same when it comes to protecting user privacy and collection of user data.

**Recommended browsers**

* Tor browser (for true anonymity browsing, not ideal for daily-driving)
* Librewolf
* Mullvad
* Brave browser
* Ungoogled chromium (with UBlock Origin)
* Helium
* Hardened Firefox & firefox ESR

**Not recommended**

* Google chrome
* Opera
* Microsoft edge

### VPN providers

While encryption ensures security a vpn provider helps us to mask identity along with the added benefits of encryption. while using a VPN our internet activity is completely hidden from Internet Service Provider.

**Recommended providers**

* Mullvad VPN
* IVPN
* ProtonVPN (have unlimited bandwidth for free)
* Windscribe VPN

**Not recommended**

* NordVPN
* Surfshark
* TurboVPN
* Private Internet Access
* Any other free VPN from playstore
* VPN provided by anti-virus softwares.

## 7. Cryptographic file encryption tools

There are tools that allow users them-self implement encryption for files. usually this tools become useful when uploading any highly confidential files to the cloud. Which provides added layer of security.

### Recommended tools

* Cryptomator
* VeraCrypt
* 7-Zip


## 8. Conclusion

No matter how much the technology is developed, security issues are always there and many malicious actors, governments and data brokers need your data. Encryption is an essential tool every individual can use to minimize or prevent this type of attacks and spying even though it is not a bulletproof solution.

---

Hope you found this article useful.

Thank you for reading.