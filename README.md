**English** | **[العربية](README.ar.md)**

# 🔎 Arabic OSINT Awesome

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Check Links](https://github.com/YOUR_USERNAME/arabic-osint-awesome/actions/workflows/links.yml/badge.svg)](https://github.com/YOUR_USERNAME/arabic-osint-awesome/actions/workflows/links.yml)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: CC0](https://img.shields.io/badge/License-CC0-lightgrey.svg)](LICENSE)

> A curated list of **open-source intelligence (OSINT)** tools and resources, with a focus on the **Arabic-speaking world (MENA)**. Every entry says what the tool does, when to use it, and where it falls short. Not a link dump.
>
> Arabic descriptions are available in **[README.ar.md](README.ar.md)**.

**Legend:** 🆓 Free · 💰 Paid · 🔑 Free with account · 🧰 Open source / CLI

## Contents

1. [Search engines and dorking](#search)
2. [Username and email lookup](#username-email)
3. [Domain, IP, and infrastructure](#infra)
4. [Social media (public data only)](#social)
5. [Image analysis and geolocation](#image-geo)
6. [Maps and satellite imagery](#maps)
7. [Leak and breach checking](#leaks)
8. [Arabic and MENA-specific sources](#mena)
9. [Learning: courses, CTFs, books, channels](#learning)
10. [Ethics and legal](#ethics)
11. [Contributing](#contributing)

---

<a id="search"></a>
## 1. Search engines and dorking

- [Google Advanced Search](https://www.google.com/advanced_search) 🆓 - A form for site, filetype, date, and language filters. Good for beginners; typing operators by hand is faster and more precise.
- [Google Hacking Database](https://www.exploit-db.com/google-hacking-database) 🆓 - Huge archive of ready-made dorks. Useful for inspiration, but mostly security-oriented rather than general investigation.
- [DorkSearch](https://dorksearch.com) 🆓💰 - Builds dork queries through a simple UI. Free tier is limited.
- [Yandex](https://yandex.com) 🆓 - Different index from Google, strong at reverse image search and Russian/Eastern European content.
- [Bing](https://www.bing.com) 🆓 - Independent index that sometimes surfaces results Google doesn't. Fewer operators.
- [Brave Search](https://search.brave.com) 🆓 - Independent index with better privacy. Handy as a second opinion.
- [DuckDuckGo](https://duckduckgo.com) 🆓 - Privacy-friendly with bangs. Less depth than Google.
- [Wayback Machine](https://web.archive.org) 🆓 - Old snapshots of websites. Not every page is archived, and owners can opt out.
- [archive.today](https://archive.ph) 🆓 - Instant snapshot of a page before it gets deleted, which preserves evidence. Access may be blocked on some networks.
- [Google Alerts](https://www.google.com/alerts) 🆓 - Email alerts for new mentions of a name or keyword. Simple and good for ongoing monitoring.

<a id="username-email"></a>
## 2. Username and email lookup

- [Sherlock](https://github.com/sherlock-project/sherlock) 🧰 - Searches a username across hundreds of sites. Expect false positives, so verify each hit manually.
- [Maigret](https://github.com/soxoj/maigret) 🧰 - Like Sherlock, but also collects info from found profiles and builds a report. Slower, richer.
- [WhatsMyName](https://whatsmyname.app) 🆓 - Web version of a community-maintained username dataset. Good when you can't install anything.
- [Namechk](https://namechk.com) 🆓 - Checks whether a name is taken across platforms. Quick first pass.
- [Holehe](https://github.com/megadose/holehe) 🧰 - Checks whether an email is registered on well-known sites. Sites change behavior, so some modules break over time.
- [Epieos](https://epieos.com) 🆓💰 - Links an email or phone to public accounts (e.g. a Google account). Results depend on the owner's privacy settings.
- [Hunter](https://hunter.io) 🔑💰 - Finds a company's email format and published addresses. Free tier has few searches.

<a id="infra"></a>
## 3. Domain, IP, and infrastructure

- [ICANN Lookup](https://lookup.icann.org) 🆓 - Official WHOIS. Most personal data is now redacted for privacy.
- [crt.sh](https://crt.sh) 🆓 - Searches published SSL certificates and reveals subdomains you didn't know existed. One of the best free sources.
- [DNSDumpster](https://dnsdumpster.com) 🆓 - Quick DNS map of a domain. Results are limited compared to paid tools.
- [SecurityTrails](https://securitytrails.com) 🔑💰 - DNS and WHOIS history. Free plan is limited.
- [ViewDNS.info](https://viewdns.info) 🆓 - DNS and reverse-IP tools in one place. Dated UI, still practical.
- [Shodan](https://www.shodan.io) 🔑💰 - Search engine for internet-connected devices. Use it for discovery only; never connect to systems you don't own.
- [Censys](https://search.censys.io) 🔑💰 - Shodan alternative focused on certificates and services. Low free quota.
- [urlscan.io](https://urlscan.io) 🆓🔑 - Scans a page and shows a screenshot and every request it makes. Great for suspicious links.
- [VirusTotal](https://www.virustotal.com) 🆓🔑 - Scans files and URLs with many engines and links related domains and IPs. Anything you upload is visible to researchers, so don't upload sensitive files.
- [BuiltWith](https://builtwith.com) 🆓💰 - Identifies the technologies a site uses. Full detail is paid.
- [Wappalyzer](https://www.wappalyzer.com) 🆓💰 - Browser extension for spotting site technologies. Faster for everyday checks.
- [BGPView](https://bgpview.io) 🆓 - Find ASNs and IP ranges for any organization. Useful to learn who owns a network.
- [Hurricane Electric BGP Toolkit](https://bgp.he.net) 🆓 - Detailed BGP, ASN, and prefix data. Good for deeper network digging.
- [IPinfo](https://ipinfo.io) 🆓💰 - Approximate location and provider for an IP. Geolocation is approximate, not exact.
- [Subfinder](https://github.com/projectdiscovery/subfinder) 🧰 - Passive subdomain discovery. Better with API keys for extra sources.
- [Amass](https://github.com/owasp-amass/amass) 🧰 - Comprehensive attack-surface mapping. Heavier and slower, but more thorough.
- [theHarvester](https://github.com/laramies/theHarvester) 🧰 - Collects emails and domains from public sources. Most sources need API keys.
- [SpiderFoot](https://github.com/smicallef/spiderfoot) 🧰 - Automates collection from many sources with a web UI. Produces a lot of data you'll need to sift.

<a id="social"></a>
## 4. Social media (public data only)

- [X Advanced Search](https://x.com/search-advanced) 🔑 - Search by date, language, and account. For Arabic content, use the language filter `lang:ar`.
- [Social Searcher](https://www.social-searcher.com) 🆓💰 - Searches public posts across several platforms. Limited coverage and a small free tier.
- [TGStat](https://tgstat.com) 🆓💰 - Stats and search for public Telegram channels. Useful for regional channels; coverage isn't complete.
- [Telepathy](https://github.com/jordanwildon/Telepathy) 🧰 - Archives and analyzes public Telegram channels and groups. Needs a Telegram API account.
- [Instaloader](https://github.com/instaloader/instaloader) 🧰 - Downloads data from public Instagram profiles. Instagram blocks heavy use.
- [InVID-WeVerify](https://www.invid-project.eu/tools-and-services/invid-verification-plugin/) 🆓 - Browser plugin for video verification: keyframes and reverse search. Essential for checking viral videos.
- [YouTube DataViewer](https://citizenevidence.amnestyusa.org) 🆓 - Shows exact upload time and thumbnails for a YouTube video, helps with reverse search.

<a id="image-geo"></a>
## 5. Image analysis and geolocation

- [Google Lens](https://lens.google.com) 🆓 - Strong reverse search for places, objects, and text inside images.
- [TinEye](https://tineye.com) 🆓💰 - Finds the earliest appearance of an image. Great for tracing origin.
- [Yandex Images](https://yandex.com/images) 🆓 - Often the best reverse image search, sometimes recognizing buildings and streets.
- [ExifTool](https://exiftool.org) 🧰 - Reads full EXIF metadata. Most platforms strip EXIF on upload, so don't always expect results.
- [FotoForensics](https://fotoforensics.com) 🆓 - ELA analysis to spot edits. Needs experience, and isn't conclusive on its own.
- [Forensically](https://29a.ch/photo-forensics) 🆓 - Browser-based image forensics toolkit, including clone detection.
- [SunCalc](https://www.suncalc.org) 🆓 - Sun direction and shadow length. Core tool for estimating time and place from shadows.
- [GeoGuessr](https://www.geoguessr.com) 🆓💰 - A game that trains your eye for country clues: roads, signs, vegetation.
- [Overpass Turbo](https://overpass-turbo.eu) 🆓 - Queries OpenStreetMap data (e.g. every gas station next to a mosque). Powerful but has a learning curve.
- [Mapillary](https://www.mapillary.com) 🆓 - Crowdsourced street imagery, covering places Street View doesn't.
- [PeakFinder](https://www.peakfinder.com) 🆓💰 - Identifies mountains from the skyline. Useful for landscape photos.
- [Wikimapia](https://wikimapia.org) 🆓 - Crowdsourced map tagging buildings and facilities. Accuracy varies by area.

<a id="maps"></a>
## 6. Maps and satellite imagery

- [Google Earth](https://earth.google.com) 🆓 - Historical imagery and 3D view. The timeline slider helps compare changes.
- [OpenStreetMap](https://www.openstreetmap.org) 🆓 - Open map, sometimes more detailed than Google. Coverage depends on volunteers.
- [Copernicus Browser](https://browser.dataspace.copernicus.eu) 🆓🔑 - Free Sentinel imagery. Resolution is about 10 m, so not suited for small details.
- [Sentinel Hub EO Browser](https://apps.sentinel-hub.com/eo-browser/) 🆓🔑 - Browse and compare satellite images across dates with analysis layers.
- [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/map/) 🆓 - Near-real-time active fire map. Useful for verifying large fires and events.
- [Zoom Earth](https://zoom.earth) 🆓 - Near-live satellite imagery and storm tracking. Low resolution.
- [FlightRadar24](https://www.flightradar24.com) 🆓💰 - Flight tracking. Long history is paid.
- [ADS-B Exchange](https://globe.adsbexchange.com) 🆓 - Unfiltered flight tracking, including some aircraft other sites hide.
- [MarineTraffic](https://www.marinetraffic.com) 🆓💰 - Ship tracking. Coverage drops when a vessel turns off AIS.
- [VesselFinder](https://www.vesselfinder.com) 🆓💰 - Alternative to MarineTraffic with basic details free.

<a id="leaks"></a>
## 7. Leak and breach checking

> For checking your own accounts and legitimate investigations. Never use leaked data to harm, extort, or access someone's accounts.

- [Have I Been Pwned](https://haveibeenpwned.com) 🆓 - Tells you if your email appeared in a known breach. The best-known tool, and privacy-respecting.
- [Intelligence X](https://intelx.io) 🔑💰 - Search engine for leaked data, darknet, and archives. Full access is paid.
- [DeHashed](https://dehashed.com) 💰 - Index of leaked data. Paid. Check the legal position in your country first.
- [TruffleHog](https://github.com/trufflesecurity/trufflehog) 🧰 - Finds leaked secrets (API keys, passwords) in code. Good for auditing your own repos.
- [GitHub Search](https://github.com/search) 🆓 - Public code search often reveals keys and internal info by accident. Use qualifiers like `org:` and `filename:`.

<a id="mena"></a>
## 8. Arabic and MENA-specific sources

This is the section most English lists lack.

### Registries and open data

- [OpenCorporates](https://opencorporates.com) 🆓💰 - Largest open company database. MENA coverage is uneven, so treat it as a starting point, not a final source.
- [ICIJ Offshore Leaks Database](https://offshoreleaks.icij.org) 🆓 - Panama Papers, Pandora Papers, and more. Includes names and companies from the region, but appearing in it isn't proof of wrongdoing.
- [OCCRP Aleph](https://aleph.occrp.org) 🔑 - Documents and records platform for investigative journalists. Very useful for tracing company networks.
- [Humanitarian Data Exchange](https://data.humdata.org) 🆓 - Humanitarian data, administrative boundaries, and indicators for MENA countries. Good for geographic and demographic context.
- [World Bank Open Data](https://data.worldbank.org) 🆓 - Economic and social indicators per country. For general context.
- [Wathq (Saudi Arabia)](https://wathq.sa) 🆓💰 - Verification services for Saudi commercial registry data. Some services are for registered entities only.
- [SaudiNIC](https://nic.sa) 🆓 - Registry for `.sa` domains. Useful for checking who owns a Saudi domain.

> 🛠️ **Contributions needed:** commercial registries, official gazettes, and domain registries for other countries (`.eg` `.ae` `.iq` `.ma` `.dz` `.tn` `.jo` `.lb` and more). If you know a reliable source, open a PR.

### Verification, archives, and documentation

- [Misbar](https://misbar.com) 🆓 - Arabic fact-checking platform. Check here to see if a claim has already been verified.
- [Fatabyyano](https://fatabyyano.net) 🆓 - Arabic fact-checking. Use it before starting from scratch.
- [Matsda2sh](https://matsda2sh.com) 🆓 - Fact-checking with a focus on Egyptian content.
- [Akhbarmeter](https://akhbarmeter.org) 🆓 - Fact-checking in Jordan and neighboring countries.
- [Verify-Sy](https://verify-sy.com) 🆓 - Fact-checking focused on Syria.
- [Syrian Archive](https://syrianarchive.org) 🆓 - Verified archive of open-source content on the Syrian conflict. A model of good archiving methodology.
- [ACLED](https://acleddata.com) 🆓🔑 - Conflict and political violence event data, coded by place and date. Essential for regional security analysis.
- [Airwars](https://airwars.org) 🆓 - Documents civilian harm from airstrikes. Open methodology you can learn from.
- [Liveuamap](https://liveuamap.com) 🆓💰 - Live event map. Sources vary, so verify each event yourself.
- [SMEX](https://smex.org) 🆓 - Reports on digital rights in the Arab region. Helps with context on censorship and blocking.
- [ARIJ](https://arij.net) 🆓 - Network of Arab investigative journalists. Guides and training material.

### Tips for searching in Arabic

1. **Try every spelling of a name.** Arabic has variants: `محمد` / `محمّد`, `أحمد` / `احمد` / `إحمد`. Hamza forms, ta marbuta (`ة`/`ه`), and alef maqsura (`ى`/`ي`) all change results.
2. **Try every Latin transliteration.** `Mohamed` `Mohammed` `Muhammad` `Mohamad`, and `Abdelrahman` `Abdul Rahman` `Abd al-Rahman`.
3. **Arabizi.** People write `7abibi` `3amr` `5aled` `9alah`. Numbers stand for letters: 2=ء 3=ع 5=خ 7=ح 9=ص. Search both forms.
4. **Restrict by country.** Use `site:.eg` `site:.sa` `site:.ae` `site:.iq` to narrow to local sites.
5. **Use the language filter.** On X: `lang:ar`. On Google: advanced settings or `&lr=lang_ar`.
6. **Dialects change the words.** The same event is described differently in Egypt, the Gulf, the Levant, and the Maghreb. Try synonyms from more than one dialect.
7. **Search with and without diacritics,** and use exact-phrase quotes `" "` when words must stay together.
8. **Place names have several forms.** `القاهرة` / `Cairo` / `Al-Qahira`, `الدار البيضاء` / `Casablanca` / `Casa`. Check historical names too.
9. **Telegram is the biggest Arabic source.** A lot of news appears there first. Search with TGStat and external engines, and archive everything because channels get deleted.
10. **Screenshot and archive immediately.** Arabic content circulating during events gets deleted fast.

<a id="learning"></a>
## 9. Learning: courses, CTFs, books, channels

- [OSINT Framework](https://osintframework.com) 🆓 - Huge taxonomy of tools. Great for exploring, but it doesn't explain tools or verify links.
- [Bellingcat Online Investigations Toolkit](https://bellingcat.gitbook.io/toolkit) 🆓 - Curated tool list with explanations from the Bellingcat team. A core reference.
- [Trace Labs](https://www.tracelabs.org) 🆓 - CTF events searching for missing persons, in cooperation with authorities. Real-world practice with real impact.
- [Gralhix](https://gralhix.com) 🆓 - OSINT and geolocation challenges with detailed write-ups. Excellent practice.
- [Sector035 - Week in OSINT](https://sector035.nl) 🆓 - Weekly newsletter on new tools and techniques. English.
- [OSINT Curious](https://osintcurio.us) 🆓 - Articles, podcast, and videos on methodology and tools.
- [IntelTechniques](https://inteltechniques.com) 🆓💰 - Tools and material from Michael Bazzell, author of *Open Source Intelligence Techniques*. The book is paid.
- [TryHackMe](https://tryhackme.com) 🔑💰 - Hands-on OSINT rooms within security learning paths. Good for beginners.

> 🛠️ **Contributions needed:** active Arabic YouTube channels, Telegram channels, and communities for OSINT. Suggest only ones you actually follow.

<a id="ethics"></a>
## 10. Ethics and legal

OSINT means collecting **publicly available** information. "Available" does not mean "fair to use any way you like."

- **Know your local law.** Cybercrime and privacy laws vary, and some in the region are strict.
- **Public data only.** Don't log into accounts, bypass protections, or impersonate anyone to deceive them.
- **Don't expose people.** Compiling private individuals' details (doxxing) can cause real harm.
- **Leaks:** checking your own accounts or doing legitimate investigations is very different from using stolen data against individuals.
- **Document your method and save your sources.** Separate confirmed facts from inference.
- **Weigh potential harm** before publishing results, especially if people could be endangered.

The tools here are for learning, verification, journalism, and lawful security research. Responsibility lies with the user.

<a id="contributing"></a>
## 11. Contributing

Contributions are welcome, especially for the **MENA section**. Read [CONTRIBUTING.md](CONTRIBUTING.md) first. In short: a tool you've personally tried, a one-to-two-line description, free or paid, and a note on its limits.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)
