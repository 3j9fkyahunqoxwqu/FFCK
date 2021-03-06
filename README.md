    [][][][][]  []  [][][][] [][][][][] [][][][][]  [][][][][]  []       []
    []              [][]  [] []         []          []      []    []   []
    [][][]      []  [][]  [] [][][]     [][][]      []      []      []
    []          []  []  []   []         []          []      []    []   []
    []          []  []    [] [][][][][] []          [][][][][]  []       [] about:config
     
    Firefox About:Config Tricks & Hardening (based on kb.mozillazine.org, 12bytes.org, user.js project)
    
    Speed up and harden your Mozilla Firefox Browser!
					==== Introduced by CHEF-KOCH ==== 
	
	
[![Matrix](https://img.shields.io/matrix/cknews:matrix.org.svg?label=CK%27s%20Technology%20News%20-%20Matrix%20Chat&server_fqdn=matrix.org&style=popout)](https://matrix.to/#/#cknews:matrix.org)
![Twitter Follow](https://img.shields.io/twitter/follow/@CKsTechNews.svg?label=Follow%20%40CKsTechNews&style=social)
[![Discord](https://discordapp.com/api/guilds/418256415874875402/widget.png)](https://discord.me/CHEF-KOCH)
[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/CHEF-KOCH)

### Project Overview

This project provides a hardened user.js (and some other files) which are designed for everyone to drag & drop into his Firefox profile folder, the process can of course be automated via scripts/programs.

* FFCK project is **not a documentation** for each about:config flag.
* FFCK project **does not believe in FUD or claims** made-up without evidence.
* FFCK project **does not explain web standards** or is designed to talk about web security policy mechanism, [Mozilla itself has an entire portal](https://developer.mozilla.org/en-US/) for this.
* FFCK project **does not care about backward-compatibility to older/outdated Browser** versions.
* FFCK project **does hope to provide a middle way between privacy and a _normal_ daily usage habit** without breaking too much.


### Project Goals

* Limit the possibilities to track the user through web analytics.
* Harden the browser against known data disclosure or code execution vulnerabilities (see _Security aspect_).
* Limit the browser from storing anything even remotely sensitive persistently.
* Harden the browser's encryption (cipher suites, protocols, trusted CAs).
* Limit possibilities to uniquely identify the browser/device using browser fingerprinting.
* Reduce the overall attack surface by disabling various features.
* Still be usable in daily use environment. 


### Privacy aspect

Several changes you can make within the Firefox options (and the invisible ones via about:config) might reducing the overall attack surface, they can be tested against several [test pages](https://github.com/CHEF-KOCH/Online-Privacy-Test-Resource-List) to check wherever they work or not. Those pages are mostly PoC pages to prove that certain things can be exploited or are vulnerable, however those changes are highly depending on the settings and Browser version and need to be constantly maintained to adopt new changes which are might coming from the Browser or new web standards itself. 


### Security aspect

The project list is not designed to secure Firefox, it is designed to bring _as much as privacy (via about:flags changes) as possible_. The project owner does not believe that the configuration increases any security aspect of the Browser, there was never a proof given that a about:config really has an impact on the overall security level of each individual config user.

Possible Problems:
* An attacker can use the open source list to find weaknesses (forgotten flags, mistakes or find other strategies to bypass it)
* The Browser itself ignores several flags or the provided options are bugged or entirely broken
* The flags are depending on the Browser source code which basically spoken means that if the source is flawed or doesn't worked as advertised an attacker can find its way around with new a Proof of concept (PoC) which might not even public available.
* About:config changes does not migrate attacks like [MITM](https://en.wikipedia.org/wiki/Man-in-the-middle_attack), data leaks, source code problems, [exploits](https://en.wikipedia.org/wiki/Exploit_(computer_security)), [0day](https://en.wikipedia.org/wiki/Zero-day_(computing)) or other spoofing attacks which might be unknown.

Archiving more security is way harder than trying to build defenses against privacy related attacks because [those two things are not the same](https://www.globalsign.com/en/blog/what-is-the-difference-between-privacy-and-security/) and the philosophy (in my opinion) must be that important problems have to be always addresses by the Browser itself without the need to change some flags/options. Stay away from ["Ultimative Firefox Privacy & Security Guides"](https://www.bestvpn.com/guides/firefox-privacy-security-guide/) those are in 99% of all cases [clickbait](https://en.wikipedia.org/wiki/Clickbait) and are very soon outdated, browser security itself is very very hard to archive if not almost impossible and needs constantly to be monitored.

