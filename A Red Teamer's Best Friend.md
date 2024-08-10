# Red Teaming Toolkit

This repository contains cutting-edge open-source security tools (OST) that will help you during adversary simulation and as information intended for threat hunter can make detection and prevention control easier. The list of tools below that could be potentially misused by threat actors such as APT and Human-Operated Ransomware (HumOR). If you want to contribute to this list send me a pull request.

---

## Table of Contents
 - [Reconnaissance](#Reconnaissance)
 - [Initial Access](#Initial-Access)
 - [Delivery](#Delivery)
 - [Situational Awareness](#situational-awareness)
 - [Credential Dumping](#credential-dumping)
 - [Privilege Escalation](#privilege-escalation)
 - [Defense Evasion](#defense-evasion)
 - [Persistence](#persistence)
 - [Lateral Movement](#lateral-movement)
 - [Exfiltration](#exfiltration)
 - [Miscellaneous](#miscellaneous)

---

## Reconnaissance
|Name|Description|URL|
|-----|-----------|----|
|RustScan|The Modern Port Scanner. Find ports quickly (3 seconds at its fastest). Run scripts through our scripting engine (Python, Lua, Shell supported).|https://github.com/RustScan/RustScan|
|Amass|In-depth Attack Surface Mapping and Asset Discovery|https://github.com/OWASP/Amass|
|gitleaks|Gitleaks is a SAST tool for detecting hardcoded secrets like passwords, api keys, and tokens in git repos.|https://github.com/zricethezav/gitleaks|
|S3Scanner|Scan for open S3 buckets and dump the contents|https://github.com/sa7mon/S3Scanner|
|cloud_enum|Multi-cloud OSINT tool. Enumerate public resources in AWS, Azure, and Google Cloud.|https://github.com/initstring/cloud_enum|
|Recon-ng|Open Source Intelligence gathering tool aimed at reducing the time spent harvesting information from open sources.|https://github.com/lanmaster53/recon-ng|
|buster|An advanced tool for email reconnaissance|https://github.com/sham00n/buster|
|linkedin2username|OSINT Tool: Generate username lists for companies on LinkedIn|https://github.com/initstring/linkedin2username|
|WitnessMe|Web Inventory tool, takes screenshots of webpages using Pyppeteer (headless Chrome/Chromium) and provides some extra bells & whistles to make life easier.|https://github.com/byt3bl33d3r/WitnessMe|
|pagodo|pagodo (Passive Google Dork) - Automate Google Hacking Database scraping and searching|https://github.com/opsdisk/pagodo|
|AttackSurfaceMapper|AttackSurfaceMapper is a tool that aims to automate the reconnaissance process.|https://github.com/superhedgy/AttackSurfaceMapper|
|SpiderFoot|SpiderFoot is an open source intelligence (OSINT) automation tool. It integrates with just about every data source available and utilises a range of methods for data analysis, making that data easy to navigate.|https://github.com/smicallef/spiderfoot|
|dnscan|dnscan is a python wordlist-based DNS subdomain scanner.|https://github.com/rbsec/dnscan|
|spoofcheck|A program that checks if a domain can be spoofed from. The program checks SPF and DMARC records for weak configurations that allow spoofing.|https://github.com/BishopFox/spoofcheck|
|LinkedInt|LinkedIn Recon Tool|https://github.com/vysecurity/LinkedInt|
|BBOT|Recursive internet scanner inspired by Spiderfoot, but designed to be faster, more reliable, and friendlier to pentesters, bug bounty hunters, and developers.|https://github.com/blacklanternsecurity/bbot|

## Initial Access

### Brute Force
|Name|Description|URL|
|-----|-----------|----|
|SprayingToolkit|Scripts to make password spraying attacks against Lync/S4B, OWA & O365 a lot quicker, less painful and more efficient|https://github.com/byt3bl33d3r/SprayingToolkit|
|o365recon|Retrieve information via O365 with a valid cred|https://github.com/nyxgeek/o365recon|
|CredMaster|Refactored & improved CredKing password spraying tool, uses FireProx APIs to rotate IP addresses, stay anonymous, and beat throttling|https://github.com/knavesec/CredMaster|

### Payload Development
|Name|Description|URL|
|-----|-----------|----|
|Ivy|Ivy is a payload creation framework for the execution of arbitrary VBA (macro) source code directly in memory.|https://github.com/optiv/Ivy|
|PEzor|Open-Source PE Packer|https://github.com/phra/PEzor|
|GadgetToJScript|A tool for generating .NET serialized gadgets that can trigger .NET assembly load/execution when deserialized using BinaryFormatter from JS/VBS/VBA scripts.|https://github.com/med0x2e/GadgetToJScript|
|ScareCrow|Payload creation framework designed around EDR bypass.|https://github.com/optiv/ScareCrow|
|Donut|Donut is a position-independent code that enables in-memory execution of VBScript, JScript, EXE, DLL files and dotNET assemblies. |https://github.com/TheWover/donut|
|Mystikal|macOS Initial Access Payload Generator|https://github.com/D00MFist/Mystikal|
|charlotte|c++ fully undetected shellcode launcher ;)|https://github.com/9emin1/charlotte|
|InvisibilityCloak|Proof-of-concept obfuscation toolkit for C# post-exploitation tools. This will perform the below actions for a C# visual studio project.|https://github.com/xforcered/InvisibilityCloak|
|Dendrobate|Dendrobate is a framework that facilitates the development of payloads that hook unmanaged code through managed .NET code.|https://github.com/FuzzySecurity/Dendrobate|
|Offensive VBA and XLS Entanglement|This repo provides examples of how VBA can be used for offensive purposes beyond a simple dropper or shell injector. As we develop more use cases, the repo will be updated.|https://github.com/BC-SECURITY/Offensive-VBA-and-XLS-Entanglement|
|xlsGen|Tiny Excel BIFF8 Generator, to Embedded 4.0 Macros in *.xls|https://github.com/aaaddress1/xlsGen|
|darkarmour|Windows AV Evasion|https://github.com/bats3c/darkarmour|
|InlineWhispers|Tool for working with Direct System Calls in Cobalt Strike's Beacon Object Files (BOF)|https://github.com/outflanknl/InlineWhispers|
|EvilClippy|A cross-platform assistant for creating malicious MS Office documents. Can hide VBA macros, stomp VBA code (via P-Code) and confuse macro analysis tools. Runs on Linux, OSX and Windows.|https://github.com/outflanknl/EvilClippy|
|OfficePurge|VBA purge your Office documents with OfficePurge. VBA purging removes P-code from module streams within Office documents.|https://github.com/fireeye/OfficePurge|
|ThreatCheck|Identifies the bytes that Microsoft Defender / AMSI Consumer flags on.|https://github.com/rasta-mouse/ThreatCheck|
|CrossC2|Generate CobaltStrike's cross-platform payload|https://github.com/gloxec/CrossC2|
|Ruler|Ruler is a tool that allows you to interact with Exchange servers remotely, through either the MAPI/HTTP or RPC/HTTP protocol.|https://github.com/sensepost/ruler|
|DueDLLigence|Shellcode runner framework for application whitelisting bypasses and DLL side-loading. The shellcode included in this project spawns calc.exe.|https://github.com/fireeye/DueDLLigence|
|RuralBishop|RuralBishop is practically a carbon copy of UrbanBishop by b33f, but all P/Invoke calls have been replaced with D/Invoke.|https://github.com/rasta-mouse/RuralBishop|
|TikiTorch|TikiTorch was named in homage to CACTUSTORCH by Vincent Yiu. The basic concept of CACTUSTORCH is that it spawns a new process, allocates a region of memory, then uses CreateRemoteThread to run the desired shellcode within that target process. Both the process and shellcode are specified by the user.|https://github.com/rasta-mouse/TikiTorch|
|SharpShooter|SharpShooter is a payload creation framework for the retrieval and execution of arbitrary CSharp source code. SharpShooter is capable of creating payloads in a variety of formats, including HTA, JS, VBS and WSF.|https://github.com/mdsecactivebreach/SharpShooter|
|SharpSploit|SharpSploit is a .NET post-exploitation library written in C#|https://github.com/cobbr/SharpSploit|
|MSBuildAPICaller|MSBuild Without MSBuild.exe|https://github.com/rvrsh3ll/MSBuildAPICaller|
|macro_pack|macro_pack is a tool by @EmericNasi used to automatize obfuscation and generation of MS Office documents, VB scripts, and other formats for pentest, demo, and social engineering assessments.|https://github.com/sevagas/macro_pack|
|inceptor|Template-Driven AV/EDR Evasion Framework|https://github.com/klezVirus/inceptor|
|mortar|evasion technique to defeat and divert detection and prevention of security products (AV/EDR/XDR)|https://github.com/0xsp-SRD/mortar|
|ProtectMyTooling|Multi-Packer wrapper letting us daisy-chain various packers, obfuscators and other Red Team oriented weaponry. Featured with artifacts watermarking, IOCs collection & PE Backdooring. You feed it with your implant, it does a lot of sneaky things and spits out obfuscated executable.|https://github.com/mgeeky/ProtectMyTooling|
|Freeze|Freeze is a payload toolkit for bypassing EDRs using suspended processes, direct syscalls, and alternative execution methods|https://github.com/optiv/Freeze|
|Shhhloader|Shhhloader is a work in progress shellcode loader. It takes raw shellcode as input and compiles a C++ stub that does a bunch of different things to try and bypass AV/EDR|https://github.com/icyguider/Shhhloader|

## Delivery
### Phishing
|Name|Description|URL|
|-----|-----------|----|
|o365-attack-toolkit|A toolkit to attack Office365|https://github.com/mdsecactivebreach/o365-attack-toolkit|
|Evilginx2|Evilginx2 is a man-in-the-middle attack framework used for phishing credentials and session cookies of any web service.|https://github.com/kgretzky/evilginx2|
|Gophish|Gophish is an open-source phishing toolkit designed for businesses and penetration testers. It provides the ability to quickly and easily setup and execute phishing engagements and security awareness training.|https://github.com/gophish/gophish|
|PwnAuth|PwnAuth a web application framework for launching and managing OAuth abuse campaigns.|https://github.com/fireeye/PwnAuth|
|Modlishka|Modlishka is a flexible and powerful reverse proxy, that will take your ethical phishing campaigns to the next level.|https://github.com/drk1wi/Modlishka|

### Watering Hole Attack
|Name|Description|URL|
|-----|-----------|----|
|BeEF|BeEF is short for The Browser Exploitation Framework. It is a penetration testing tool that focuses on the web browser|https://github.com/beefproject/beef|

## Command and Control

### Remote Access Tools (RAT)
|Name|Description|URL|
|-----|-----------|----|
|Cobalt Strike|Cobalt Strike is software for Adversary Simulations and Red Team Operations.|https://cobaltstrike.com/|
|SpecterInsight|SpecterInsight is a cross-platform, post-exploitation command and control framework based on .NET for red team engagements, threat emulation, and training. It provides a variety of obfuscated payloads out-of-the-box and makes avoiding detection a core feature. Command outout is returned in JSON format and exported to ELK for analysis of operations with pre-built dashboards.|https://practicalsecurityanalytics.com/specterinsight/|
|Brute Ratel C4|Brute Ratel is the most advanced Red Team & Adversary Simulation Software in the current C2 Market.|https://bruteratel.com/|
|Empire|Empire 5 is a post-exploitation framework that includes a pure-PowerShell Windows agent, and compatibility with Python 3.x Linux/OS X agents.|https://github.com/BC-SECURITY/Empire|
|PoshC2|PoshC2 is a proxy aware C2 framework used to aid penetration testers with red teaming, post-exploitation and lateral movement.|https://github.com/nettitude/PoshC2|
|Koadic|Koadic C3 COM Command & Control - JScript RAT|https://github.com/zerosum0x0/koadic|
|merlin|Merlin is a cross-platform post-exploitation Command & Control server and agent written in Go.|https://github.com/Ne0nd0g/merlin|
|Mythic|A cross-platform, post-exploit, red teaming framework built with python3, docker, docker-compose, and a web browser UI.|https://github.com/its-a-feature/Mythic|
|Covenant|Covenant is a .NET command and control framework that aims to highlight the attack surface of .NET, make the use of offensive .NET tradecraft easier, and serve as a collaborative command and control platform for red teamers.|https://github.com/cobbr/Covenant|
|shad0w|A post exploitation framework designed to operate covertly on heavily monitored environments|https://github.com/bats3c/shad0w|
|Sliver|Sliver is a general purpose cross-platform implant framework that supports C2 over Mutual-TLS, HTTP(S), and DNS.|https://github.com/BishopFox/sliver|
|SILENTTRINITY|An asynchronous, collaborative post-exploitation agent powered by Python and .NET's DLR|https://github.com/byt3bl33d3r/SILENTTRINITY|
|Pupy|Pupy is an opensource, cross-platform (Windows, Linux, OSX, Android) remote administration and post-exploitation tool mainly written in python|https://github.com/n1nj4sec/pupy|
|Havoc|Havoc is a modern and malleable post-exploitation command and control framework, created by @C5pider.|https://github.com/HavocFramework/Havoc|
|NimPlant|A light first-stage C2 implant written in Nim and Python|https://github.com/chvancooten/NimPlant|
|SharpC2|SharpC2 is a Command & Control (C2) framework written in C#. It consists of an ASP.NET Core Team Server, a .NET Framework implant, and a .NET MAUI client.|https://github.com/rasta-mouse/SharpC2|

### Staging
|Name|Description|URL|
|-----|-----------|----|
|pwndrop|Self-deployable file hosting service for red teamers, allowing to easily upload and share payloads over HTTP and WebDAV.|https://github.com/kgretzky/pwndrop|
|C2concealer|A command line tool that generates randomized C2 malleable profiles for use in Cobalt Strike.|https://github.com/FortyNorthSecurity/C2concealer|
|FindFrontableDomains|Search for potential frontable domains|https://github.com/rvrsh3ll/FindFrontableDomains|
|Domain Hunter|Checks expired domains for categorization/reputation and Archive.org history to determine good candidates for phishing and C2 domain names|https://github.com/threatexpress/domainhunter|
|RedWarden|Flexible CobaltStrike Malleable Redirector|https://github.com/mgeeky/RedWarden|
|AzureC2Relay|AzureC2Relay is an Azure Function that validates and relays Cobalt Strike beacon traffic by verifying the incoming requests based on a Cobalt Strike Malleable C2 profile.|https://github.com/Flangvik/AzureC2Relay|
|C3|C3 (Custom Command and Control) is a tool that allows Red Teams to rapidly develop and utilise esoteric command and control channels (C2).|https://github.com/FSecureLABS/C3|
|Chameleon|A tool for evading Proxy categorisation|https://github.com/mdsecactivebreach/Chameleon|
|Cobalt Strike Malleable C2 Design and Reference Guide|Cobalt Strike Malleable C2 Design and Reference Guide|https://github.com/threatexpress/malleable-c2/|
|redirect.rules|Quick and dirty dynamic redirect.rules generator|https://github.com/0xZDH/redirect.rules|
|CobaltBus|Cobalt Strike External C2 Integration With Azure Servicebus, C2 traffic via Azure Servicebus|https://github.com/Flangvik/CobaltBus|
|SourcePoint|SourcePoint is a C2 profile generator for Cobalt Strike command and control servers designed to ensure evasion.|https://github.com/Tylous/SourcePoint|
|RedGuard|RedGuard is a C2 front flow control tool,Can avoid Blue Teams,AVs,EDRs check.|https://github.com/wikiZ/RedGuard|
|skyhook|A round-trip obfuscated HTTP file transfer setup built to bypass IDS detections.|https://github.com/blackhillsinfosec/skyhook|
|GraphStrike|Cobalt Strike HTTPS beaconing over Microsoft Graph API|https://github.com/RedSiege/GraphStrike|

### Log Aggregation
|Name|Description|URL|
|-----|-----------|----|
|RedELK|Red Team's SIEM - tool for Red Teams used for tracking and alarming about Blue Team activities as well as better usability in long term operations.|https://github.com/outflanknl/RedELK|
|Elastic for Red Teaming|Repository of resources for configuring a Red Team SIEM using Elastic.|https://github.com/SecurityRiskAdvisors/RedTeamSIEM|
|RedEye|RedEye is a visual analytic tool supporting Red & Blue Team operations|https://github.com/cisagov/RedEye|

## Situational Awareness
### Host Situational Awareness
|Name|Description|URL|
|-----|-----------|----|
|AggressiveProxy|AggressiveProxy is a combination of a .NET 3.5 binary (LetMeOutSharp) and a Cobalt Strike aggressor script (AggressiveProxy.cna). Once LetMeOutSharp is executed on a workstation, it will try to enumerate all available proxy configurations and try to communicate with the Cobalt Strike server over HTTP(s) using the identified proxy configurations.|https://github.com/EncodeGroup/AggressiveProxy|
|Gopher|C# tool to discover low hanging fruits|https://github.com/EncodeGroup/Gopher|
|SharpEDRChecker|Checks running processes, process metadata, Dlls loaded into your current process and the each DLLs metadata, common install directories, installed services and each service binaries metadata, installed drivers and each drivers metadata, all for the presence of known defensive products such as AV's, EDR's and logging tools.|https://github.com/PwnDexter/SharpEDRChecker|
|Situational Awareness BOF|This Repo intends to serve two purposes. First it provides a nice set of basic situational awareness commands implemented in BOF.|https://github.com/trustedsec/CS-Situational-Awareness-BOF|
|Seatbelt|Seatbelt is a C# project that performs a number of security oriented host-survey "safety checks" relevant from both offensive and defensive security perspectives.|https://github.com/GhostPack/Seatbelt|
|SauronEye|SauronEye is a search tool built to aid red teams in finding files containing specific keywords.|https://github.com/vivami/SauronEye|
|SharpShares|Multithreaded C# .NET Assembly to enumerate accessible network shares in a domain|https://github.com/mitchmoser/SharpShares|
|SharpAppLocker|C# port of the Get-AppLockerPolicy PowerShell cmdlet with extended features. Includes the ability to filter and search for a specific type of rules and actions.|https://github.com/Flangvik/SharpAppLocker/|
|SharpPrinter|Printer is a modified and console version of ListNetworks|https://github.com/rvrsh3ll/SharpPrinter|
