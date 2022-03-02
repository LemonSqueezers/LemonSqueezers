                                          The Lemon Squeezers Journal
2 Mar 2022                                                                                                              Issue #6


Arti 0.1.0 Released!

2-3-22: Tor's embed'able client in Rust. today, Tor reached 0.1.0 milestone: this means that Tor now 
considers Arti's high-level APIs to be "mostly stable", and ready for experimental embedding in other projects. 
(Tor doesn't promise no API breakage, but Tor doesn't break your high-level APIs without a good reason.) The 1.0.0 milestone, 
scheduled for September, will represent an even stronger API commitment.
the primary new features are Tor's builder API for constructing TorClient instances, and the ability to create 
unbootstrapped and bootstrap-on-demand TorClient instances. These features make it easier to create a "lazy" 
TorClient that bootstraps itself in the background the first time it's used: Tor provided some example code to show you how.
Tor has also replaced it's error APIs.  Previously, it exposed a huge mass of APIs from lower-level crates, and encouraged 
dependencies on unstable lower-level error types. Now the error details are hidden, and there is instead an explicitly supported 
ErrorKind type that programs can use to see what type of error occurred. (You can still access the low-level information by 
enabling an optional trait, if you really want to.)

Sources:
https://blog.torproject.org/arti_010_released/
----------------------------------------------------------------------------------------------------------------------------------
Anonymous leaks database of the Ministry of Economic Development of Russia

The anonymous collective has leaked the Ministry of Economic Development of Russia's database.

Sources:
https://twitter.com/YourAnonOne/status/1498685800241934342?cxt=HHwWjMC9lfCys8wpAAAA
----------------------------------------------------------------------------------------------------------------------------------
LemonSqueezers celebrates International Pancake Day!

1-3-22: Today is Pancake Day, where everyone celebrates the most delicious breakfast
treat!
----------------------------------------------------------------------------------------------------------------------------------
Debunking the Dark Web

1-3-22: Many people think that the dark web is huge, when actually there are only 60,000 websites there.
other lies and myths:
1. It is full of drug markets
most sites there are mundane.
2. There are mystery boxes
No. they are all scams.
3. It is illegal
It depends on where you are and what you are viewing.
----------------------------------------------------------------------------------------------------------------------------------
1-3-22: Hacker group Modified Elephant APT found injecting 'evidence' into computers

in Sept. 2021, A hacker group named EGoManiac wasplanting incriminating evidence 
on the systems of journalists to justify arrests by the Turkish National Police. A similiar 
hacker group called ModifiedElephant APT does similiar things.
The objective of ModifiedElephant is long-term surveillance that at times concludes with the 
delivery of ‘evidence’—files that incriminate the target in specific crimes—prior to conveniently coordinated 
arrests. In the last decade, they have targeted Activists, human rights defenders, journalists, academics, 
and law professionals. They send phishing emails to the victims. Their primary delivery mechanism is malicious 
Microsoft Office document files weaponized to deliver the malware of choice at the time. 
The specific payloads changed over the years and across different targets. However, some notable trends remain.

In mid-2013, the actor used phishing emails containing executable file attachments with fake double extensions (filename.pdf.exe).
After 2015, the actor moved on to less obvious files containing publicly available exploits, such as .doc, .pps, 
.docx, .rar, and password protected .rar files. These attempts involved legitimate lure documents in .pdf, .docx, and 
.mht formats to captivate the target’s attention while also executing malware.
In 2019 phishing campaigns, ModifiedElephant operators also took the approach of providing links to files hosted 
externally for manual download and execution by the target.
As first publicly noted by Amnesty in reference to a subset of this activity, the attacker also made use of 
large .rar archives (up to 300MB), potentially in an attempt to bypass detection.
Observed lure documents repeatedly made use of CVE-2012-0158, CVE-2014-1761, CVE-2013-3906,
CVE-2015-1641 exploits to drop and execute their malware of choice.
The spearphishing emails and lure attachments are titled and generally themed around topics relevant to the 
target, such as activism news and groups, global and local events on climate change, politics, 
and public service. A public deconstruction of two seperate 2014 phishing emails was shared by Arsenal Consulting in early 2021.
ModifiedElephant continually made use of free email service providers, like Gmail and Yahoo, to conduct their campaigns.
The phishing emails take many approaches to gain the appearance of legitimacy. This includes fake body content 
with a forwarding history containing long lists of recipients, original email recipient lists with many seemingly 
fake accounts, or simply resending their malware multiple times using new emails or lure documents. Notably, in specific 
attacks, the actor would be particularly persistent and attempt to compromise the same individuals multiple times in a single day.

By reviewing a timeline of attacker activity, we can observe clear trends as the attacker(s) rotate infrastructure over the years.
The malware most used by ModifiedElephant is unsophisticated and downright mundane, and yet it has proven sufficient for their 
objectives–obtaining remote access and unrestricted control of victim machines. The primary malware families deployed were NetWire 
and DarkComet remote access trojans (RATs). Both of these RATs are publicly available, and have a long history of abuse by threat 
actors across the spectrum of skill and capability.

One particular activity revolves around the file Ltr_1804_to_cc.pdf, which contains details of an assassination plot 
against Prime Minister Modi. A forensic report by Arsenal Consulting showed that this file, one of the more incriminating pieces of 
evidence obtained by the police, was one of many files delivered via a NetWire RAT remote session that we associate with ModifiedElephant. 
Further analysis showed how ModifiedElephant was performing nearly identical evidence creation and organization across multiple unrelated 
victim systems within roughly fifteen minutes of each other.
ModifiedElephant also sent multiple phishing emails containing both NetWire and Android malware payloads at the same time. 
The Android malware is an unidentified commodity trojan delivered as an APK file (0330921c85d582deb2b77a4dc53c78b3).

While the Android trojan bears marks of being designed for broader cybercrime, its delivery at the same time as 
ModifiedElephant Netwire samples indicates that the same attacker was attempting to get full coverage of the target on 
both endpoint and mobile. The full report contains further details about the Android Trojan.
Attributing an attacker like ModifiedElephant is an interesting challenge. At this time, we possess significant evidence of what 
the attacker has done over the past decade, a unique look into who they’ve targeted, and a strong understanding of their technical objectives.

We observe that ModifiedElephant activity aligns sharply with Indian state interests and that there is an observable correlation 
between ModifiedElephant attacks and the arrests of individuals in controversial, politically-charged cases.

Sources:
https://www.sentinelone.com/labs/modifiedelephant-apt-and-a-decade-of-fabricating-evidence/
----------------------------------------------------------------------------------------------------------------------------------
The Cake Story

1-3-22: owner: yeah! this cake is the best here!
cashier: be careful, he has a gun
*owner ignores warning*
*cake put in freezer*
owner: lets eat it!
*cake gets half-eaten*
owner: WHAT?!
*cake runs inside fridge*
*cake eats another cake*
*cake pulls out gun*
owner: RUN!
*owner gets killed*
cake: yay! another victim!
*cake eats owner-guy*

Moral of the Story: do not let a cake have a gun
----------------------------------------------------------------------------------------------------------------------------------
Steam deck is here... and its bad

1-3-2022: From the terrible compatibility to the fact that it costs 30117.28 Rupees here 
in India so most gamers wont be able to play it right now. of course, valve may make 
it cheaper but it does have another issue: it is not available in most countries
at launch.

Sources:
https://www.steamdeck.com/en/
Linus Tech Tips on YT
----------------------------------------------------------------------------------------------------------------------------------
After 2 years, people forgot how to climb trees

after covid began, society and parents told us that we should climb huge trees and fall off. 
One of the risks of climbing trees is thorns. it may impale you and even contain bacteria. 

Sources: 
https://www.ashevilletreeremovals.com/the-dangers-of-tree-climbing/

Idea: CarZim on Discord
----------------------------------------------------------------------------------------------------------------------------------
What are the uses of cocoa beans in our daily life?

Cocoa beans are used to make coffee and chocolate. But high amounts 
of coffee cause insomnia and chocolate causes diabetes. So drink at maximum 2 cups of coffee
and eat chocolate once per week.
Sources:
https://kidadl.com/fun-facts/learn-all-about-amazing-cocoa-beans-and-its-various-uses
Idea: Poatato
----------------------------------------------------------------------------------------------------------------------------------
why is the amount of blue candles in the world increasing these days

According to Chinese culture, blue candle's lighter will seek harmony, truth, creativity, and guidance.

Sources
https://chi-nese.com/everything-you-need-to-know-about-spiritual-candle-colors/
Idea: poatato on Discord
----------------------------------------------------------------------------------------------------------------------------------
Suggest a Idea!

If you have a idea DM Spcycake2 #4353, in the discussions section of the repo. or email me at cortex96@tutanota.com or buttertheidiot@gmail.com.
----------------------------------------------------------------------------------------------------------------------------------
New Windows 11 build 22563

The build is available is ARM. Not every build microsoft releases will have
as many new features as last week’s build. However, this build includes a few new features for Users
to try out as Microsoft rolls them out including a tablet-optimized taskbar experience, some
improvements to content in Widgets, and a new Notifications group policy for IT admins in education which may
be bad for under-age social media kids. Microsoft also have some notable changes and improvements in this build 
including improvements for File Explorer, support for Microsoft Edge tabs in snap 
assist and ALT + TAB, and support for Emoji 14.0.
"with bringing together the widgets and news feed experiences as a dynamic blended feed containing 
both widgets and news content. This should make it easier for you to discover and engage with new widgets
and news content through your feed. With a dynamic feed there’s less of a burden on you to curate the canvas 
on your own, but you’ll still be able to pin your favorite Widgets to the top if you want." says Microsoft

Sources

https://blogs.windows.com/windows-insider/2022/02/24/announcing-windows-11-insider-preview-build-22563/
----------------------------------------------------------------------------------------------------------------------------------
What happened to Windows 9?

Microsoft says that 7 ate 9 so they released 10 instead said a representative 
----------------------------------------------------------------------------------------------------------------------------------
Russia-Ukraine war causes crypto stocks to fall

almost all cryptocurrencies have fallen in value as Russians invade in Kyiv. only 17 cryptos has increased in value
----------------------------------------------------------------------------------------------------------------------------------

Anonymous Intercepts russian military communications

Russian military communications got intercepted on 
the 26th of February at 4220 KHz USB.

Sources:
https://twitter.com/DeepNetAnon/status/1497433491105062914
----------------------------------------------------------------------------------------------------------------------------------
Anonymous declares war on Russia

The hacker group anonymous has declared war on Russia. So far they have
hacked military installations in Russia and leaked emails and passwords, mess with 
maritime traffic data and make it look like Putin's yacht had crashed into
Ukraine's snake island, then changed its destination to Hell on Saturday 
and take down the Russian governments website down 11 hours ago at time of 
writing and Russian TV got hacked.

sources: 
Seytonic on youtube
@AnonTV on Twitter
----------------------------------------------------------------------------------------------------------------------------------
Hacker group Corvid founded

A hacker collective was founded on 9 Feb, according to the founder,
"start a hacking/programming collective" and "If anyone has any interest in joining Email me at crow16815291@protonmail.com"
The founder (crow16815291) made the group on Nova BBS's hacking board/newsgroup. the group's intentions are unknown. 
----------------------------------------------------------------------------------------------------------------------------------
Tor 11.5a4 Alpha released

on 18 Feb, Tor released a update which Updated Go to 1.17.6, Pick up obfsproxy 0.0.12. 
most of the update were bug fixes.
----------------------------------------------------------------------------------------------------------------------------------
How to Disable Windows Parental Control

1. type services in the search bar
2. search for Family Options
3. select properties from the context menu
4. set start to disabled
5. Yay!
----------------------------------------------------------------------------------------------------------------------------------
How to Spoof MAC

1. Go to View network connections in control panel
2. select properties after right clicking Wifi
3. click configure
4. go to advanced
5. click network address
6. add your own MAC (eg. 000000000000)
----------------------------------------------------------------------------------------------------------------------------------
Windows 11 area unresponsive bug

in windows 11, sometimes, when you hover over the search box, a area of the screen
is unresponsive to clicks. to fix this bug, you need to kill explorer by typing taskkill /f explorer.exe and 
pressing enter. after that type start explorer and press enter again to execute the command.

Archives: https://raw.githubusercontent.com/FrankEnderman/LemonSqueezers/main/LArchive.old
use Tor: torproject.org/download

----------------------------------------------------------------------------------------------------------------------------------
(c) Copyright 2022, Spicycake

Copy any text on this website as long as you credit.

Github's finest newspaper
