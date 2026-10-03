---
title: Jigsaw — 2 Communication (AS Level)
syllabus: 9618 (2026)
topic: 2.1 Networks including the internet
---

# Jigsaw — 2 Communication

Syllabus content for **9618 Topic 2: Communication → 2.1 Networks including the internet**, rebuilt bullet by bullet, with every tested angle mapped onto it.

**Legend**

> [!success] Already examined in 9618
> Tested in a 9618 paper (2021 onwards). Latest question ID given.

> [!warning] 9608 only (not yet in 9618)
> Tested under the old 9608 syllabus, still inside the 9618 syllabus wording. Fair game — just untested in the current series. Latest 9608 question ID given.

> [!info] Not yet tested — inference
> In syllabus, not yet asked in either series (or only asked in a much narrower form). Justification given.

> [!abstract] From the Save My Exams notes
> Content the SME revision notes teach that is not covered by any past question above. Detail worth knowing, but weigh it against the mark schemes — SME sometimes goes beyond what Cambridge credits.

---

## 2.1.1 Show understanding of the purpose and benefits of networking devices

> [!note] Reading of this bullet
> This is about the **benefits of connecting computers into a network** — sharing, central management, communication — *not* the benefits of switches/routers as hardware. Hardware purpose is covered by the "hardware that is used to support a LAN" and "role and function of a router" bullets below.

> [!success] Benefits of connecting computers to a LAN
> Sharing of files/data, sharing of resources (hardware/software), communication between devices, central management (backup, security). `9618_s23_qp_12_sc_1.a`

> [!info] Drawbacks / costs of networking computers rather than standalone
> Never asked as a stand-alone "give two drawbacks of networking" — but every other benefit bullet in this topic (cloud, wireless, P2P, subnetting) has a paired drawbacks question, so the symmetry is overdue. Expect: cost of hardware/cabling, single point of failure, malware spreads across the network, needs a network manager, security exposure.

> [!info] Justify networking in a given scenario
> The syllabus says "purpose **and** benefits", and 9618 loves "justify your choice" stems (`w21_qp_11_sc_8.a`, `w21_qp_12_sc_3.b.i`). A scenario asking *why this business should network its standalone machines* is a natural 3–4 mark extension.

> [!abstract] Definition of a network
> Two or more interconnected devices (computers, printers, servers) set up to share resources, exchange data and communicate. The **purpose** is resource sharing, communication and collaboration.

> [!abstract] Further benefits of networking
> Shared peripherals reduce cost; **network software licences are cheaper than individual licences**; access to reliable central data (file server); **a network manager can control access rights and internet usage**. The licensing and access-rights points do not appear in any mark scheme here but are standard credited answers.

> [!abstract] Drawbacks of networking (the untested half, filled in)
> Expensive setup (cabling, servers); large networks need skilled administration; server failure affects everyone; **malware or hacking spreads to the whole network**; security risk increases when connected to a wider WAN. This is the concrete answer set for the `!info` drawbacks gap above.

---

## 2.1.2 Show understanding of the characteristics of a LAN and a WAN

> [!success] Describe the characteristics of a LAN
> Small geographical area; privately owned / dedicated infrastructure; can be wired or wireless. `9618_w25_qp_12_sc_5.a`

> [!success] Describe the characteristics of a WAN
> Large geographical area; external/public infrastructure; non-dedicated hardware. `9618_w24_qp_13_sc_9.a`

> [!success] Differences between a LAN and a WAN
> Geographical area, physical vs virtual connections, data transfer rate, ownership (private vs public), security. `9618_s25_qp_12_sc_6.a`

> [!success] Identify LAN or WAN for a scenario, with justification
> e.g. a school networking one building → LAN, because small area and no leased external transmission media. `9618_w21_qp_11_sc_8.a`

> [!info] WLAN as a named term
> 9618 examines wireless LANs only through the wired/wireless bullet, never by the term WLAN. The syllabus notes name WiFi explicitly, so "state what is meant by a WLAN / give one benefit of a WLAN over a wired LAN" is a cheap 1–2 marker Cambridge has not yet used.

> [!info] MAN / intranet / extranet style distractors
> Not in 9618 wording, so unlikely to be asked directly — flagged only so you do not waste revision time on it.

> [!abstract] Quantified scale, and WAN as a collection of LANs
> LAN ≈ under 1 mile, all hardware owned by the organisation. WAN ≈ over 1 mile, and is **a collection of LANs joined together, connected via routers**, using hardware not owned by the organisation (e.g. telephone lines owned by telecoms companies). The "WAN = joined LANs, linked by routers" framing is not in any mark scheme but explains the ownership and media mark points.

> [!abstract] Typical transmission media per network type
> LAN: unshielded twisted pair (UTP), fibre optic, or Wi-Fi. WAN: fibre optic, telephone lines, satellite. Useful for linking this bullet to the wired/wireless bullet in a scenario answer.

> [!abstract] WLAN — the detail behind the untested term
> A LAN where devices connect wirelessly rather than by cable; extra hardware (**WAPs / hotspots**) is added so users can connect by Wi-Fi.
> **Advantages:** connect anywhere in range of a WAP without extra wiring; works indoors and out; more WAPs easily added to extend coverage or user count; wireless access to peripherals.
> **Disadvantages:** limited coverage, worsened by walls and structures; bandwidth suffers in high-traffic areas; interference from other devices; signals can be intercepted.

---

## 2.1.3 Explain the client-server and peer-to-peer models of networked computers

> [!success] Roles of the devices in a client-server model (applied to a scenario)
> Identify the server + description (receives/processes requests, stores data); identify the client + description (sends request, waits, outputs response). `9618_s25_qp_13_sc_3.c`

> [!success] Explain why a given scenario *is* a client-server model
> Web server stores the data, browser is the client, sends requests over the internet, server acts and returns results. `9618_s25_qp_13_sc_3.c`

> [!success] Key features of a peer-to-peer network
> All computers of equal status; each provides access to resources/data (distributed); each responsible for its own security. `9618_s21_qp_11_sc_4.a`

> [!success] Drawbacks of a peer-to-peer network
> Reduced security (only as secure as the weakest machine), no central backup, no central management of files/software, individual machines slow down, all machines must be switched on. `9618_s21_qp_11_sc_4.b`

> [!warning] Benefits of the client-server model
> Files and resources centralised, security is centrally managed, username/password control, centralised backup, clients can be cheaper machines. Tested repeatedly in 9608 but **never** as a 9618 "benefits of client-server" question. `9608_w15_qp_13_sc_7.a.ii`

> [!warning] Describe the client-server model *in general* (definition, not scenario)
> "At least one computer serves, others are clients, the server provides services which clients request." 9618 always wraps this in a scenario. `9608_w15_qp_13_sc_7.a.i`

> [!warning] Types of server and their purposes
> File server, print server, proxy server, web server, application server, mail server. `9608_s19_qp_12_sc_1.d`

> [!warning] Client-server applied to a non-web scenario (supermarket tills, bank)
> The self-checkout/barcode scenario and the bank-login scenario. 9618 has used banking (`s24_qp_11_sc_5.a`) but the "describe using an example" phrasing with a marks cap for no application is 9608's. `9608_w19_qp_11_sc_4.a.i`

> [!info] Benefits of peer-to-peer over client-server
> 9618 has asked P2P drawbacks and client-server roles, but never the P2P *advantages* (no expensive server, no single point of failure, cheap/easy to set up, no dedicated admin). The obvious missing quarter of the 2×2.

> [!info] Justify choosing client-server vs peer-to-peer for a given situation
> The syllabus notes explicitly say *"justify the use of a model for a given situation"* — 9618 has tested "explain why this is client-server" but never asked candidates to **choose and defend** a model. Highest-probability new question in this bullet.

> [!info] Subnetwork models within the client-server bullet
> The notes say "roles of the different computers within the network **and subnetwork models**" — subnetting has only ever been tested under the IP bullet, never linked back to network models here.

> [!abstract] Drawbacks of the client-server model
> **Single point of failure** — if the server goes down, services are unavailable; expensive to set up and maintain, often needing a dedicated team. Neither point appears in a 9618 mark scheme, and they are the natural counterweight to the 9608 "benefits of client-server" question above.

> [!abstract] Benefits of peer-to-peer, spelled out
> Easy and cheap to set up, no administrative staff needed; no dependency on a central server; data shared directly between machines. Fills the `!info` gap above.

> [!abstract] When each model is used
> Client-server suits **larger organisations** needing centralised control, reliability and security. Peer-to-peer suits **home networks, small businesses and file sharing**. The deciding factors are security, cost, ease of setup and maintenance requirements — that four-factor list is the shape of the "justify the use of a model" answer the syllabus notes demand.

> [!abstract] Thin-client and thick-client can be hardware *or* software
> A thin-client may be a device or an application; likewise thick. **Thin-client examples:** Google Docs / Microsoft 365, remote desktop (Citrix, Chrome Remote Desktop), supermarket POS terminals fetching prices and stock from a central server. **Thick-client examples:** installed Photoshop or Word, standalone games, a school laptop running applications offline. The mark schemes only ever use abstract characteristics, so having a concrete example ready is what turns a characteristic into an applied mark.

> [!abstract] Thin vs thick — the comparison table the bullet asks for
> Dependence on server (permanent connection vs independent) · processing power (server's vs its own) · offline behaviour (does not work vs functions offline) · best for (centralised control and low-cost devices vs performance, flexibility and offline access) · network type (part of a LAN/WAN vs may connect but is not reliant). This is the answer set for the untested "differences between them" question.

---

## 2.1.4 Show understanding of thin-client and thick-client and the differences between them

> [!success] Characteristics of a thin-client, applied to a scenario
> Data not stored on client; reliant on server / network connection; few local resources needed; performs minimal processing. `9618_s24_qp_12_sc_3.b`

> [!success] Describe what is meant by a thick-client model
> Server performs minimal/some processing; clients do most of their own processing, resources installed locally. `9618_s23_qp_12_sc_1.e`

> [!success] Role of the computers when thin-clients are used in a client-server model
> Server performs **all** processing and/or storage; clients **only** send requests and display returned results. `9618_s23_qp_13_sc_2.c`

> [!info] Direct thin vs thick comparison table
> Both halves have been tested separately but never side by side, even though the syllabus bullet ends *"and the differences between them"*. A "complete the table / give two differences" question is the literal reading of the bullet and has not appeared.

> [!info] Benefits and drawbacks of thin-client for an organisation
> Only characteristics have been asked. Benefits (cheap terminals, central updates/security, easy to add clients) and drawbacks (server is a single point of failure, heavy network dependence, server load) are untested and are exactly the "implications" style 9618 uses elsewhere.

---

## 2.1.5 Show understanding of the bus, star, mesh and hybrid topologies

> [!success] Draw / complete a star topology diagram
> All devices connected directly to the central device (switch) and no other connections; server connected to the switch. `9618_w25_qp_12_sc_5.b`

> [!success] Draw a labelled topology for a described office (computers, server, printers, switch, router)
> `9618_s25_qp_12_sc_6.d`

> [!success] Describe how packets are transmitted between two hosts in a star topology
> Sender sends packets to the switch; switch checks the destination address; forwards **only** to the intended recipient. `9618_w25_qp_12_sc_5.c`

> [!success] Describe what is meant by a mesh topology
> All computers connected to at least one other device; multiple routes between devices; computers act as relays passing packets towards the destination. `9618_s23_qp_13_sc_2.b.i`

> [!success] Advantages of mesh over bus
> More routes if a line fails; improved security (not one main line); fewer collisions; new nodes added without interruption. `9618_s23_qp_13_sc_2.b.ii`

> [!success] Advantage of star over bus, with expansion
> More resilient (no single cable); higher performance / fewer collisions; easier to add nodes; easier fault finding. `9618_w23_qp_11_sc_2.d`

> [!success] Match statements to bus / star / mesh (tick table)
> Central device = star; central cable = bus; multiple paths = mesh; robust to line failure = star & mesh; most collisions = bus. `9618_s24_qp_11_sc_8.a`

> [!success] Identify the topology of a described network and justify
> e.g. home network where all devices connect only to the router → star. `9618_w21_qp_12_sc_3.b.i`

> [!info] Hybrid topology
> **Named in the syllabus bullet and never tested in either series.** Star and mesh dominate; bus appears as the contrast. Expect "describe what is meant by a hybrid topology" or a scenario (multi-site office: star within buildings, mesh between them) asking you to identify and justify it. This is the single biggest gap in the topic.

> [!info] Packet transmission in a bus or mesh topology
> Only the star version has been asked (twice). The notes say *"understand how packets are transmitted between two hosts for a given topology"* — bus (all devices see the packet, only the addressed one accepts it) and mesh (relayed via multiple possible routes) are the same question with a different word.

> [!info] Drawbacks of mesh / star, or advantages of bus
> Every topology question so far is worded in favour of star or mesh. Untested: cost and cabling complexity of full mesh, star's dependence on the central device, bus being cheap and simple for a small network.

> [!abstract] Bus topology — terminators and how devices read the cable
> All devices share one **bus cable, terminated at each end**; the terminators stop the signal bouncing back and causing errors. Each device *listens* to the electrical signals on the cable, checks every packet for its own address, and ignores packets not addressed to it. **This is the bus answer to the untested "how are packets transmitted in a given topology" question**, and terminators are never mentioned in any mark scheme in this topic.
> **Advantages:** cheap and easy — one cable; does not depend on a central switch or server. **Disadvantages:** low security (data visible to all devices); slow, collision-prone; a cable break kills the whole network.

> [!abstract] Star topology — the central device changes the behaviour
> A star with a **switch** sends traffic only to the addressed device; a star with a **hub** broadcasts to all devices, and each device accepts or ignores based on the address. Every 9618 star question assumes a switch, so this distinction is the hidden variable in "describe how packets are transmitted in a star topology".
> **Disadvantages:** the central switch is a single point of failure — if it fails, every device loses network access; installation cost of the switch and extra cabling.

> [!abstract] Mesh — full vs partial, and routing vs flooding
> **Full mesh** = every computer connected to every other. **Partial mesh** = a practical, cheaper alternative and what is used in reality. Packets travel by either **routing** (devices hold routing logic and send by the shortest route) or **flooding** (packets sent to all devices with no routing logic, which can cause performance problems). Mark schemes only credit "computers act as relays" — the routing/flooding distinction and the term *partial mesh* appear nowhere in either series, but they are the mesh answer to "how are packets transmitted".
> **Disadvantages:** lots of hardware, cabling and switches; high set-up cost; hard to scale. Common real use is IoT — wearables and smart home devices.

> [!abstract] Hybrid topology — the content for the topic's biggest gap
> A mix of two or more topologies (bus + star, star + mesh, …), typically used **when separate existing networks must be joined**. Worked example: a trust takes over three schools running bus, star and mesh respectively and links them as one hybrid network — each site keeps its own setup, new sites can be added without redesigning everything.
> **Advantages:** combines the strengths of each topology; flexible — different parts optimised for different needs; scalable; a failure in one part need not affect the rest. **Disadvantages:** complex to design; expensive (more hardware and maintenance); harder to troubleshoot because different parts follow different rules.

---

## 2.1.6 Show understanding of cloud computing

> [!success] Benefits of storing data using cloud computing
> Free for limited amounts; no need for personal storage devices; access from any computer with an internet connection; backup/recovery included; easy sharing; capacity easily increased. `9618_w25_qp_12_sc_8.a.i`

> [!success] Drawbacks of using cloud computing
> Needs an internet connection; no control over backups/security; slow upload/download; provider downtime; compatibility issues; limited free storage; more expensive long term. `9618_w25_qp_12_sc_8.a.ii`

> [!success] Define the term private cloud
> Dedicated/bespoke services or storage on a remote server available only to that company. `9618_s24_qp_13_sc_5.a.i`

> [!success] Benefits of private cloud over public cloud
> Not reliant on a third party; greater control over security/privacy and backup; storage tailored/scalable to requirements. `9618_s24_qp_13_sc_5.a.ii`

> [!success] Explain why a company would use a public cloud
> Content must be available to anyone / over the internet; willing to share infrastructure; more economic. `9618_w23_qp_13_sc_3.a.i`

> [!success] Disadvantages of public cloud compared to a LAN server
> Loss of control (data on someone else's infrastructure), reliance on external agency for backups/security, needs reliable internet, recurring costs vs one-off LAN cost. `9618_w23_qp_13_sc_3.a.ii`

> [!success] Identify the type of cloud in a hardware diagram
> `9618_w22_qp_13_sc_7.a`

> [!info] Define public cloud / directly compare public vs private
> Private has been *defined*; public has only ever been reasoned about. A "define public cloud" or "state two differences between public and private cloud" one-to-two marker is trivially writable and untested.

> [!info] Cloud as a service model (software as well as storage)
> `w22_qp_13_sc_7.a` accepted applications running on the cloud, and `s21_qp_12_sc_5.c` opens with "Seth accesses both software **and** data using cloud computing" — but no question has yet asked about accessing *software/applications* on the cloud (benefits of not installing locally, automatic updates, device independence).

> [!info] Drawbacks of a private cloud
> The benefits of private over public are examined; the flip side (cost of infrastructure, company must manage/maintain it, less scalable) has not been.

> [!abstract] Cloud computing splits into cloud *storage* and cloud *software*
> **Cloud storage** — long-term data storage on remote servers in data centres (HDDs, increasingly SSDs), reachable only over the internet (a WAN). e.g. Google Drive, Dropbox, OneDrive.
> **Cloud software** — applications hosted and managed remotely, used on demand, with the provider handling maintenance, upgrades and security, usually on a monthly or yearly subscription. e.g. Google Docs, Microsoft 365, Adobe Creative Cloud.
> Every 9618 cloud question so far is about storage. This is the framing behind the `!info` gap on software-as-a-service above.

> [!abstract] Cloud software — benefits and drawbacks
> **Benefits:** usable on any device with internet; no installation; automatic updates and patching; no specialist IT staff needed; plan easily scaled up or down; provider-managed firewalls and encryption; works across laptop/tablet/phone.
> **Drawbacks:** will not work properly offline; performance depends on connection speed; ongoing subscription cost; data privacy — your data sits on the provider's servers; less control over when updates happen; **you remain legally responsible for personal data even when it is hosted elsewhere**; features may be reduced compared with the locally installed version.

> [!abstract] Extra cloud-storage benefits not in any mark scheme
> No need to buy expensive storage hardware; no need to hire specialist IT staff; **eco-friendly — centralised data centres are more efficient than millions of local servers**; data backed up across multiple servers; built-in security features such as encryption and multi-factor authentication.

> [!abstract] Public vs private cloud, dimension by dimension
> Ownership (third-party provider vs the company itself) · access (shared with other organisations vs restricted to one) · cost (cheaper through shared infrastructure vs company pays for hardware, maintenance and staff) · control (less vs full) · security (relies on the provider's measures vs custom policies and full oversight). Examples: public — Google Drive, Microsoft 365; private — a company intranet or internal cloud servers. This is the ready-made answer to the untested "state two differences between public and private cloud".

---

## 2.1.7 Show understanding of the differences between and implications of the use of wireless and wired networks

> [!success] Advantages of a wireless network compared to a wired network
> Mobility (no physical connection), no cabling so easier/cheaper to set up, easier to add devices, many device types can connect. `9618_w25_qp_13_sc_4.a`

> [!success] Drawback of using a wireless network
> Less secure; slower transmission speed; interference; signal degrades without repeaters/boosters. `9618_w25_qp_13_sc_4.b`

> [!success] Identify and describe transmission media (copper, fibre-optic, radio/microwave)
> Fibre optic → pulses of light; radio waves/microwaves → electromagnetic waves on different frequencies. `9618_w24_qp_13_sc_9.b`

> [!success] Satellites: advantage and disadvantages vs copper cable
> Advantage: not fixed to a location, reaches remote areas. Disadvantages: high latency, expensive extra equipment, affected by weather, slower than fixed-line broadband, needs line of sight. `9618_w22_qp_13_sc_7.b`

> [!success] Benefits of offering both wired and wireless connections
> Some devices only support one; wired gives better performance/less interference/secure transmission; wireless gives mobility and multiple/own devices. `9618_s23_qp_13_sc_2.d`

> [!success] Choose wired or wireless for a use case and justify
> Streaming/gaming → wired: higher bandwidth, less latency, more reliable, more secure. `9618_s21_qp_11_sc_4.c.ii`

> [!warning] Benefits of fibre-optic over copper cable
> Less interference; signal degrades less / needs less boosting; more secure (harder to tap); greater bandwidth / faster. Only ever described generically in 9618 ("transmits data as pulses of light"). `9608_w19_qp_11_sc_4.c.i`

> [!warning] Drawbacks of fibre-optic over copper cable
> Higher installation cost; specialists needed; difficult to terminate; fibres break when bent; transmits in one direction only. `9608_w19_qp_11_sc_4.c.ii`

> [!warning] Benefits of copper cable
> Cheaper to install, more flexible/easier to install, easier to terminate, expertise widely available. `9608_w15_qp_13_sc_6`

> [!warning] Match communication media to their features (fibre / radio / copper / satellite tick-or-line table)
> Twisted pair vs coaxial, light pulses, wireless transmission, least interference, fastest medium. `9608_s18_qp_11_sc_1`

> [!warning] Detailed wireless drawbacks with expansion
> Interception of packets, bandwidth shared and reduced as devices join, interference from obstacles, limited range/attenuation needing repeaters, higher latency. 9618 has only asked for **one** unexpanded drawback. `9608_s21_qp_12_sc_9.b`

> [!info] Microwaves as a distinct medium
> Named in the syllabus notes alongside radio waves and satellites, but only ever accepted as an alternative in a "radio waves / microwaves" mark point. A question naming microwave links specifically (line of sight, high bandwidth, point-to-point) is available.

> [!info] Twisted pair vs coaxial copper
> 9608 used it as a tick-box distractor; 9618 has never mentioned coaxial. Low probability, but it sits inside "characteristics of copper cable".

> [!abstract] Wired networks — advantages and disadvantages as a pair
> **Advantages:** fast data transfer; better physical security; high range (up to ~100 m) and less susceptible to interference. **Disadvantages:** no portability — location limited by the cable; cost of extra cabling per new device; **safety — cables are trip hazards and must be routed along walls or under floors**. The safety point appears in no mark scheme but is a legitimate "implication of use".

> [!abstract] Wireless — Bluetooth alongside Wi-Fi
> The two common wireless standards are **Wi-Fi** (devices communicate with a WAP, standalone or built into a router/switch) and **Bluetooth** (typically a direct connection between two devices — headphones, controllers, keyboards). Bluetooth is named nowhere in the syllabus notes or any mark scheme, so treat it as background, not a target answer.
> Wireless range relies on signal strength to the WAP and can be obstructed (up to ~90 m) — the concrete figure behind the "signal degrades" mark point.

> [!abstract] The three transmission media compared properly
> **Twisted pair** — electrical signals, LAN use (desktops, printers, servers in homes/offices), duplex, slowest of the three, prone to electromagnetic interference, cheap.
> **Coaxial** — electrical signals, originally telecoms voice/landline, adapted to carry WAN traffic, degrades over time limiting range, suffers interference, lower bandwidth than fibre, medium cost.
> **Fibre optic** — light signals, high-speed WANs and modern internet backbones, highest bandwidth and speed, **no interference so the most secure for sensitive data**, minimal degradation over long distances (spans cities and countries), expensive, full duplex.
> This table is the answer bank for both the 9608-only fibre-vs-copper questions above and the syllabus's "characteristics of copper cable, fibre-optic cable".

---

## 2.1.8 Describe the hardware that is used to support a LAN

> [!success] Describe the role of a switch in a network
> Stores MAC addresses of connected devices; receives packets; forwards directly to the intended recipient; central point of connection; enables devices to communicate. `9618_s25_qp_12_sc_6.e`

> [!success] Purpose of switch, WAP and bridge in a table
> WAP → lets devices connect to the central device using radio/WiFi signals, connects wireless-enabled devices to a wired network. Bridge → connects two LANs/segments using the **same protocol**. `9618_w23_qp_11_sc_2.b`

> [!success] Functions of a Wireless Network Interface Card (WNIC)
> Interface/antenna to the wireless network; receives analogue radio waves and converts to digital; checks incoming transmissions for the correct MAC/IP and ignores others; encrypts/decrypts; converts digital to analogue and sends via the antenna. `9618_w21_qp_11_sc_8.c`

> [!success] Identify devices that physically connect computers to the rest of the network
> Router, switch, hub. `9618_w21_qp_11_sc_8.b`

> [!success] Identify which LAN device the router attaches to, with a reason
> Server (processes requests / firewall / proxy) or switch (connected to all computers, shares access). `9618_w22_qp_12_sc_10.b.i`

> [!success] Identify hardware from a labelled network diagram
> `9618_s25_qp_12_sc_6.d`

> [!warning] Purpose of a gateway, and router vs gateway
> Both regulate traffic between two networks and forward packets; a router connects networks using the **same** protocol, a gateway connects networks using **different** protocols. 9608 asked this repeatedly; 9618 has only ever let "acts as a gateway" appear as one bullet inside a router answer. `9608_s20_qp_11_sc_8.c`

> [!warning] Purpose of a modem as LAN/internet-connecting hardware
> To connect devices to the internet over a telephone line. (9618 has tested modems only under the *internet* hardware bullet.) `9608_s20_qp_12_sc_7.a`

> [!info] NIC (wired), repeater, cables — described in their own right
> The syllabus notes list *switch, server, NIC, WNIC, WAP, cables, bridge, repeater*. The **wired NIC** has only ever been mentioned in a question stem, and the **repeater** appears only as a mark point inside a wireless-drawback answer. "Describe the function of a repeater / a NIC" is an untested 2-marker sitting explicitly in the notes.

> [!info] Role of the server as LAN hardware
> Listed first in the notes and drawn in every diagram, but never asked as "describe the role of the server in a LAN" — despite the switch getting exactly that treatment in `s25_qp_12_sc_6.e`.

> [!info] Switch vs hub
> "Hub" is accepted in `w21_qp_11_sc_8.b` but never examined. A "give one difference between a switch and a hub" (hub broadcasts to all, switch forwards only to the recipient) follows directly from the switch mark scheme.

> [!abstract] Hub — the "dumb" device
> Connects multiple devices, but passes anything received on one connection to **all** other connections. Two consequences: unnecessary traffic (worse the more devices there are) and a **security concern**, since every device receives every packet. Cheaper than a switch. This is the content for the switch-vs-hub gap above, and it also explains the hub variant of a star topology.

> [!abstract] The switch's lookup table
> A switch holds a **lookup table mapping ports to MAC addresses**. On receiving a packet it reads the destination MAC, finds it in the table, and forwards the packet out of the corresponding port only. The mark scheme for `s25_qp_12_sc_6.e` credits "stores the MAC addresses of devices connected to it" — the port↔MAC table and the word *packet switching* are the mechanism behind that mark.

> [!abstract] The server as LAN hardware
> A powerful computer providing services or resources to clients: stores and manages files, hosts websites, controls printer access, runs applications. Built to handle many simultaneous requests and stay on 24/7, usually kept in a dedicated room or data centre, running a specialist OS (Windows Server, Linux). May be local to the LAN or reached remotely over a WAN. Types: file, print, web, mail. **Fills the `!info` gap on "describe the role of the server in a LAN".**

> [!abstract] NIC — the wired one, described in its own right
> Historically a card in a motherboard slot, now usually built in; provides a dedicated full-time connection, converting the computer's data into a network-ready format and sending/receiving packets. Has a built-in Ethernet port for an Ethernet cable, and a **unique MAC address identifying the device on the network**. Fills the wired-NIC gap above and links directly to the switch lookup table and Ethernet frames.

> [!abstract] WAP — bridge between wired and wireless, and range extender
> Lets wireless devices join a wired network, acting as a bridge between the wired and wireless parts. Often built into a wireless router but may be a separate device in larger networks. Uses radio signals, follows Wi-Fi standards (802.11ac, 802.11ax), and **extends the range of the wireless network in large buildings**. The range-extension role is credited nowhere but is why multiple WAPs exist in a school or office.

> [!abstract] Bridge — filtering, not just joining
> Connects two network segments so two LANs act as one larger network, and **filters traffic by checking MAC addresses** to decide whether data should cross, which reduces overall traffic. The 9618 mark scheme only credits "connects two LANs with the same protocol"; the filtering behaviour is the reason a bridge is used rather than a plain cable.

> [!abstract] Repeater
> Receives a weak signal and **retransmits it at full strength**, boosting or regenerating it so data can travel long distances without loss of quality; used for both wired and wireless, e.g. Wi-Fi range extenders. Named in the syllabus notes and never examined — this is the whole answer.

---

## 2.1.9 Describe the role and function of a router in a network

> [!success] Function of a router in a network
> Receives packets; analyses the destination IP address; forwards towards the destination using the routing table; maintains/updates the routing table; finds the most efficient route; allocates private IP addresses; implements a firewall; NAT. `9618_w23_qp_11_sc_2.a`

> [!success] Role of routers in transmission of data **through the internet**
> Receives packets from the internet, analyses destination IP, forwards using the routing table, finds the most efficient route. `9618_s24_qp_12_sc_3.c.i`

> [!success] Identify three functions of a router in a home network
> `9618_w21_qp_12_sc_3.b.ii`

> [!success] Tick table — is this task performed by the router?
> Receives packets ✓; finds the IP address of a URL ✗ (that is DNS); directs each packet to **all** devices ✗; stores IP/MAC addresses of attached devices ✓. `9618_s21_qp_11_sc_4.c.i`

> [!success] How data is transmitted between two devices via the router
> Data goes to the router, carries the recipient's address, router determines destination using a routing table, transmits only to the recipient. `9618_w23_qp_12_sc_7.b.ii`

> [!warning] Router vs gateway (as a router question)
> Router = same protocol, gateway = different protocols; both connect networks and forward packets. `9608_s19_qp_12_sc_1.c`

> [!info] The routing table itself
> Named in almost every mark scheme but never the subject of a question. "Describe what is stored in a routing table / how a router uses it to choose a route" is a clean 2–3 marker.

> [!info] NAT explained rather than named
> NAT appears as an accepted mark point in `w23_qp_11_sc_2.a` only. Explaining *how* NAT lets many private addresses share one public address is untested and links this bullet to the public/private IP bullet below.

> [!abstract] Packet header vs payload, and hops
> A packet has a **header** (control information, including the sender's and recipient's IP addresses) and a **payload** (the actual data). The router reads the header to determine the destination. A packet may pass through several routers before arriving — **each router-to-router pass is called a hop**. Neither "payload" nor "hop" appears in any mark scheme in this topic, but they are the precise vocabulary for the credited "forwards the packet towards its destination" points.

> [!abstract] The routing table, described
> The router looks the destination IP up in a **routing table of known networks** to decide which network to send the packet to next, then forwards it. Three-step cycle: receive and analyse header → look up in routing table → forward. Repeated by every router until delivery. This is the content for the `!info` routing-table gap above.

> [!abstract] The router's additional functions
> A router commonly also provides wireless networking, a **built-in firewall**, switch capabilities, assignment of IP addresses to LAN devices, and **filtering of incoming traffic by IP address, port number or protocol type**. A router joining a LAN to a WAN has a **public IP address assigned by the ISP**, and it is that address other routers use to direct packets to the network.

---

## 2.1.10 Show understanding of Ethernet and how collisions are detected and avoided

> [!success] Describe what is meant by Ethernet
> A protocol (suite) for data transmission over wired/cabled connections; uses CSMA/CD; data transmitted in frames; each frame has source and destination addresses and error-checking data. `9618_s23_qp_12_sc_1.d`

> [!success] How collisions are detected and managed on a bus network (CSMA/CD)
> Workstations listen to the channel and send only when idle; on collision, transmission is aborted and a jamming signal is sent; random wait time before retransmitting; wait time increases with repeated collisions. `9618_w25_qp_12_sc_5.d`

> [!success] Tasks performed by devices under CSMA/CD
> Monitor the channel; transmit only when idle; detect collision and stop/jam; calculate a random back-off time; retransmit; increase the random time on repeated collisions. `9618_w23_qp_12_sc_7.c`

> [!success] Drawbacks of using CSMA/CD
> Random time increases so waiting can be unbounded; constant jamming can block sending; no prioritisation of nodes; high power consumption; only suitable for short distances; not scalable. `9618_s24_qp_13_sc_5.c.ii`

> [!info] Why collisions happen at all
> Only ever a sub-point inside `w22_qp_11_sc_8` ("more than one computer on the same transmission medium"). A short "explain why collisions occur in a bus network but not in a star network with a switch" ties this bullet to topologies and has not been asked.

> [!info] Ethernet frame structure
> The mark scheme for `s23_qp_12_sc_1.d` credits "data transmitted in frames, each with source/destination address and error-checking data" — but no question has yet asked candidates to **describe the contents of an Ethernet frame** directly.

> [!info] CSMA/CA, or collision avoidance in wireless
> The bullet says "detected **and avoided**". Everything tested so far is CD (detection). CA is not named in the syllabus, so treat this as low-probability — but "how are collisions *avoided*" (listen before transmit, switched full-duplex links) is a legitimate reading of the wording.

> [!abstract] What Ethernet actually controls
> Ethernet is a protocol governing **wiring, data transmission and data encapsulation** — a wired networking standard for LANs. The "encapsulation" framing is what ties the protocol to the frame structure below and is not wording any mark scheme uses.

> [!abstract] The Ethernet frame, field by field
> **Preamble** — a bit sequence that synchronises communication between devices · **Destination MAC address** · **Source MAC address** · **EtherType / Length** — the type of data or the payload size · **Payload** — the actual data · **FCS (Frame Check Sequence)** — error detection to check the data arrived correctly.
> `s23_qp_12_sc_1.d` credits only "frames have source and destination addresses and error-checking data". This is the full structure behind the `!info` gap above — and note *FCS* is the named field behind "error checking data", and the source/destination MACs are the same addresses the switch stores in its lookup table.

---

## 2.1.11 Show understanding of bit streaming

> [!success] State what is meant by bit streaming
> Continuous ordered flow of bits over a communication path. `9618_s24_qp_11_sc_2.e.i`

> [!success] Explain how data is transferred using real-time bit streaming
> Transmitted continuously as a series of bits; uploaded to a media server; users download from it; server sends data to a buffer on the user's device; buffer covers the speed difference; recipient views from the buffer. `9618_s25_qp_11_sc_2.a`

> [!success] Differences between real-time and on-demand bit streaming
> Real-time is direct from source, on-demand is pre-recorded; real-time cannot be re-watched or paused; real-time plays continually, on-demand downloads in sections. `9618_s24_qp_11_sc_2.e.ii`

> [!success] Why video is compressed before real-time streaming
> Video is data-intensive; reduces file size → less bandwidth → less buffering → participants stay in sync and low-bandwidth users can join. `9618_s25_qp_11_sc_2.b.i`

> [!success] How bit streaming is used in a real-time video conference
> `9618_w24_qp_13_sc_9.c`

> [!warning] How buffering prevents the video pausing (on-demand)
> Needs high-speed broadband; data streamed to a buffer; buffering stops pausing; as the buffer empties it refills so viewing is continuous; playback runs a few seconds behind receipt. 9618 credits "buffer" points but has never set the *why doesn't it pause* question. `9608_w16_qp_13_sc_6`

> [!warning] Benefits of bit streaming (vs downloading the whole file)
> No wait for the whole file; no need to store large files locally; on-demand playback; no specialist software beyond the browser. `9608_w15_qp_13_sc_1.b.i`

> [!warning] Problems of bit streaming
> Stops/hangs on slow broadband or inadequate buffer capacity; no internet means no access; may need specific software. `9608_w15_qp_13_sc_1.b.ii`

> [!warning] Identify real-time vs on-demand for a described scenario, with justification
> e.g. a recorded video sent to colleagues to watch later → on-demand. `9608_w19_qp_12_sc_6.e.ii`

> [!info] Importance of bit rate and broadband speed
> The syllabus notes name this explicitly: *"importance of bit rates broadband speed on bit streaming"*. 9618 has only touched it sideways through compression. A direct "explain why a high bit rate is needed / what happens when broadband speed is lower than the bit rate" question is squarely in the notes and untested in the current series.

> [!info] Bit streaming of audio rather than video
> Every question in both series uses video. Nothing in the syllabus restricts it to video; music/podcast streaming is the same answer in a new wrapper.

> [!abstract] Bit rate — definition and trade-off
> **Bit rate is the amount of data transmitted in a given unit of time** (usually per second). Higher bit rate → higher quality (HD/4K), sharper image and sound, but more bandwidth used and a larger buffer needed. Lower bit rate → pixelation and blurriness, especially in fast movement, but less bandwidth; a smaller buffer suffices, though buffering is more frequent on a poor connection. **This is the content for the "importance of bit rates" line in the syllabus notes that neither series has examined.**

> [!abstract] Broadband speed — the second named factor
> High-speed broadband supports higher bit rates, several devices streaming at once, HD/4K, smooth playback with minimal buffering, and real-time uses like gaming and video calls. Slow or restricted broadband cannot sustain a high bit rate, forces lower resolution, causes frequent buffering and interruptions, and struggles with live or interactive services.

> [!abstract] Adaptive bitrate
> Streaming platforms **adjust the bit rate dynamically based on network performance** — this is how on-demand streaming copes with a variable connection while real-time streaming cannot. It is the mechanism underneath the credited "on-demand can handle delays thanks to buffering" contrast, and the term itself appears in no mark scheme.

> [!abstract] Real-time vs on-demand — extra contrast points
> Latency (real-time needs low delay to feel live; on-demand tolerates delay through buffering) · connection (real-time needs a strong steady connection; on-demand adapts quality) · examples (live sport, live news, **online gaming, video calls** vs Netflix, YouTube). Online gaming and video calls as real-time examples do not appear in the mark schemes but are exactly the scenarios 9618 wraps questions in.

---

## 2.1.12 Show understanding of the differences between the WWW and the internet

> [!success] Explain whether an activity uses the internet, the WWW, or both
> Webmail → both: internet because data travels on the infrastructure, WWW because a website stored on a web server is accessed. `9618_s21_qp_11_sc_4.d`

> [!warning] Explain the difference between the WWW and the internet directly
> Internet = global infrastructure / interconnected networks, uses TCP/IP. WWW = collection of interlinked multimedia pages/documents stored on web servers, written in HTML, transferred using HTTP, located by URLs, viewed in a browser. **Only one 9618 question exists in this whole bullet (2021)** — the plain "distinguish between them" version is 9608's. `9608_s16_qp_13_sc_6.a`

> [!warning] True/false statement + justification ("the internet and the WWW are the same thing")
> `9608_s18_qp_11_sc_5.b`

> [!info] This is the thinnest-covered bullet in the whole topic
> One 9618 question since 2021, five years ago. Treat everything here as live: definition of each, protocols used by each (TCP/IP vs HTTP), and "is this activity internet, WWW or both" for non-web services (email client, VoIP, online gaming, file transfer).

> [!abstract] The internet is itself a WAN
> "Inter**net**work" — a global network of networks, and **the most well-known WAN**; it is the *infrastructure* that provides connectivity to the WWW, using TCP/IP. This one sentence links this bullet back to the LAN/WAN bullet and is the cleanest way to justify "she is using the internet because data travels on the infrastructure".

> [!abstract] The WWW, described in full
> A collection of websites and web pages accessed *using* the internet: interconnected documents and multimedia files stored on web servers worldwide, retrieved and displayed by a web browser, transferred using **HTTP and HTTPS**. Created in 1989 by Tim Berners-Lee. The HTTPS pairing and the historical detail appear in no mark scheme — the protocol contrast (TCP/IP vs HTTP) is the part that earns marks.

---

## 2.1.13 Describe the hardware that is used to support the internet

> [!success] Use of modems and dedicated lines when transmitting over the internet
> Modem → converts digital to analogue for transmission down phone lines and back again. Dedicated line → direct/private connection, therefore faster transmission. `9618_s25_qp_11_sc_2.c`

> [!success] Role of the PSTN in transmission of data through the internet
> Consists of many different types of communication line; digital data may need converting to analogue; duplex transmission (both directions at once); communication passes through different switching centres/ISPs. `9618_s24_qp_12_sc_3.c.ii`

> [!success] How data is transmitted using the cell phone network
> Land split into cells for maximum line of sight; each cell has a tower with an antenna that receives and transmits; data passes between tower and phone; wireless using low-power radio frequencies; multiple devices share a tower simultaneously. `9618_s25_qp_12_sc_6.b`

> [!success] Identify the device that connects a laptop to the internet (from a diagram)
> Router. `9618_w22_qp_13_sc_7.a`

> [!warning] Benefit and drawback of installing a dedicated line
> Benefit: faster / more consistent speed / improved security. Drawback: expensive to set up and maintain; disruption leaves no alternative route. 9618 has asked what a dedicated line *is*, never whether to install one. `9608_s19_qp_12_sc_1.b.ii`

> [!warning] PSTN circuit behaviour vs internet-based transmission (tick table)
> PSTN: dedicated channel for the duration of the call, connection maintained throughout, lines active in a power outage. Internet: connection only in use while sound is transmitted, uses encoding and compression. `9608_s15_qp_12_sc_5.a`

> [!warning] Identify two pieces of internet-connecting hardware with purposes (router / gateway / modem / NIC)
> `9608_s20_qp_12_sc_7.a`

> [!info] The ISP
> Drawn in the `w22_qp_13_sc_7.a` diagram and named in the PSTN mark scheme, but never defined or explained in either series. "State the role of an Internet Service Provider" is an easy untested marker.

> [!info] Comparing the four internet-supporting technologies
> The notes list *modems, PSTN, dedicated lines, cell phone network* together. Each has been tested alone; a question asking you to choose the appropriate one for a scenario (rural site, mobile workforce, high-security link between two offices) has not appeared and matches 9618's "justify your choice" habit.

> [!abstract] Modem = modulator–demodulator
> The name itself explains the credited answer: it **modulates** digital signals into analogue to send over telephone or cable lines and **demodulates** analogue back into digital. Connection technologies it serves: DSL, cable, dial-up. Used to send and receive data over long distances on traditional communication lines.

> [!abstract] PSTN — origin and the copper-to-fibre transition
> Built after the invention of the telephone to carry voice over copper wires, then adapted for internet access as demand grew; used to connect devices and LANs between towns and cities. **Traditional copper lines are progressively being replaced with fibre optic**, giving higher bandwidth and faster transfer. That transition is not in any mark scheme but explains why "the PSTN consists of many different types of communication line" is a credited point.

> [!abstract] Dedicated lines — named types and speeds
> T1 (up to ~1.54 Mbps), T3 (up to ~45 Mbps), fibre-optic (gigabit speeds). **Always active and not shared with other users**, unlike the PSTN — hence faster and more reliable, and suited to video conferencing, cloud computing and large file transfers. The "always on, not shared" contrast is the sharpest way to express the credited "direct/private connection".

> [!abstract] Cellular networks — handover and generations
> The network is divided into cells, each served by a **cell tower / base station**; a device connects to the nearest tower, and **as the user moves the device automatically switches to the next closest tower — this is handover**. Carries voice, SMS and mobile data. Generations: 2G (calls and texts), 3G (mobile internet, video calling), 4G (fast browsing and streaming), 5G (very high speed, low latency). The `s25_qp_12_sc_6.b` mark scheme covers cells, towers and radio signals but **never mentions handover or the generations**.

---

## 2.1.14 Explain the use of IP addresses in the transmission of data over the internet

### Format of an IP address (IPv4 and IPv6)

> [!success] Complete a description of IPv4 / IPv6 format
> IPv4: four groups of 8-bit numbers separated by full stops, 32 bits total. IPv6: eight groups of 4 hexadecimal digits separated by colons, 128 bits, consecutive groups of zeros replaced by a double colon. `9618_s25_qp_12_sc_6.c`

> [!success] Differences between IPv4 and IPv6
> 4 groups vs 8 groups; denary vs hexadecimal; 0–255 vs 0–FFFF; 32 bits vs 128 bits. `9618_s24_qp_11_sc_8.b.ii`

> [!success] Explain why a given address is not IPv6 / is invalid
> Dotted notation rather than colons; only four groups; 32-bit not 128-bit; group value above 255. `9618_w25_qp_11_sc_7.b`

> [!success] Number of bits needed to store an IPv4 / IPv6 address (tick table)
> 32 and 128. `9618_w25_qp_13_sc_2.a`

> [!warning] Give an example of a valid IPv4 address
> `9608_s19_qp_12_sc_1.a.i`

> [!warning] Judge several addresses as valid/invalid with reasons, including hexadecimal IPv4 forms
> Non-hex characters, values above 255/FF, wrong number of groups, more than one double colon. 9618 has done this once for a single address; 9608 ran whole tables of them. `9608_s16_qp_12_sc_7.b`

> [!warning] State why IPv6 is needed
> The number of addresses required exceeds the number available under IPv4. **Never asked in 9618.** `9608_s19_qp_12_sc_1.a.ii`

> [!warning] State what IP stands for / the purpose of an IP address
> Internet Protocol; gives each device a unique identifier so data reaches the correct destination. `9608_w18_qp_12_sc_2.b`

> [!info] Converting or compressing an IPv6 address by hand
> Both series only ever *describe* the double-colon rule. Applying it — rewriting `2001:0db8:0000:0000:0000:ff00:0042:8329` in shortened form, or spotting why two double colons are ambiguous — is a natural Paper 1 step up and links to hexadecimal in Topic 1.

> [!abstract] What an IP address is *for*
> A unique identifier given to devices communicating over the internet, making it possible to deliver data to the right device. **A device that moves to a different network gets a different IP address** — the clearest way to express "IP addresses are dynamic".

> [!abstract] The address-space numbers behind "why IPv6"
> IPv4 gives just over 4 billion addresses (2³²) — not enough for 7+ billion people with several devices each. IPv6 gives 2¹²⁸, enough for over a billion unique addresses per person on the planet. `9608_s19_qp_12_sc_1.a.ii` credits the reason in words; these are the figures that make the argument concrete, and neither series quotes them.

### Subnetting

> [!success] Purpose of subnetting in a network
> Divides the network into smaller networks; reduces traffic/congestion; traffic travels only where necessary; hides complexity; easier maintenance. `9618_w24_qp_13_sc_9.d.ii`

> [!success] Reasons/benefits of subnetting with expansion
> Security (devices do not receive unintended data, a compromised device does not expose the whole network); easier management and fault isolation; easier expansion / more addresses; better performance and less congestion. `9618_w23_qp_12_sc_7.b.iii`

> [!success] The two parts of an IP address in a subnetwork
> Network ID and host ID; each subnetwork has a different network ID; every device in a subnetwork shares the network ID but has a unique host ID. `9618_s23_qp_13_sc_2.e`

> [!success] Use a subnet mask to identify the network ID and host ID
> `255.0.0.0` on `10.10.12.1` → network ID 10. `255.255.255.0` on `192.168.12.4` → host ID 4. `9618_w22_qp_13_sc_7.c.ii`

> [!info] Drawbacks of subnetting
> Benefits have been asked at least four times across w22–w24; the cost/complexity side (planning overhead, wasted addresses, routing between subnets needed) has never been asked. Given how heavily this bullet is examined, the inverted version is due.

> [!info] Working with a subnet mask beyond reading off a byte
> Only the trivial `255.0.0.0` / `255.255.255.0` cases have appeared. A mask that does not fall on a byte boundary, or asking how many hosts a mask allows, is within "use of subnetting in a network".

> [!abstract] Subnetting — framing and one extra benefit
> "Each subnet works like a mini-network within the main network." Alongside the examined benefits (less traffic, better performance, security, easier management), SME adds **improved organisation — grouping devices by department or function**. That organisational point appears in no mark scheme but is a defensible "aids day-to-day management" expansion.

### Public, private, static and dynamic

> [!success] Describe static and public IP addresses
> Static → does not change each time a device connects. Public → assigned to a device so it is visible on the internet. `9618_w25_qp_11_sc_7.a`

> [!success] Complete a table of all four types with descriptions
> Public / private / static / dynamic. `9618_w23_qp_12_sc_7.d`

> [!success] Purpose of a router's public and private IP addresses
> Public → so the router is visible to the internet/WAN. Private → so the router is identified to computers within the LAN. `9618_w24_qp_13_sc_9.d.i`

> [!success] State what is meant by a static private IP address
> Does not change, **and** can only be used within the LAN. `9618_s24_qp_13_sc_5.d`

> [!success] Why a router has a public IP address
> To be visible to and accessible by other devices on the internet. `9618_s24_qp_11_sc_8.b.i`

> [!success] Match each IP address type to its description (drawing lines)
> `9618_s21_qp_12_sc_5.d`

> [!warning] Two differences between a public and a private IP address
> Private known only within the LAN; public allocated by the ISP, private by the router; public unique across the internet, private unique only within the LAN; private more secure. 9618 tests the terms **separately** but has never set the head-to-head difference question. `9608_s21_qp_11_sc_9.a`

> [!warning] Why the computers on a LAN do not have public IP addresses
> Improved security (not visible outside), no internet presence needed per machine, only the router needs to be externally visible, reduces the number of public addresses needed. `9608_s20_qp_13_sc_1.c`

> [!warning] NAT is necessary for a private address to reach the internet directly
> `9608_w18_qp_11_sc_2.b.ii`

> [!warning] The private address ranges
> `10.0.0.1–10.255.255.254`, `172.16.0.1–172.31.255.254`, `192.168.0.1–192.168.255.254`. Appears as a 9608 mark point only. `9608_s16_qp_12_sc_7.c`

> [!info] Why a device would be given a static rather than a dynamic address
> Both terms are defined constantly; the *reason for choosing one* (a server or printer must be found at a fixed address; dynamic conserves addresses and suits transient devices) has never been asked, despite the syllabus notes saying "difference between a static IP address and a dynamic IP address".

> [!abstract] DHCP
> SME names **DHCP (Dynamic Host Configuration Protocol)** as the server that automatically allocates dynamic addresses from a pool of available addresses. It is **not named anywhere in the 9618 syllabus and appears in no mark scheme in either series** — know it as the mechanism, but answer in the syllabus's own words ("assigned by the router", "changes each time the device connects") rather than leaning on the acronym.

> [!abstract] Which devices get which type of address
> **Public:** devices needing a constant internet presence — web servers, email servers; globally unique, directly reachable from anywhere. **Private:** LAN devices assigned by the router — laptops, phones, printers; not routable on the internet, which improves security.
> **Static:** devices needing a consistent address — websites, remote access services, email and file servers; no management needed once set. **Dynamic:** devices where a fixed address is unnecessary — laptops, smartphones, guest devices.
> **This is the answer to the untested "why would a device be given a static rather than a dynamic address"** — it is decided by whether the device must be *found* at a known address.

> [!info] How an IP address is associated with a device on a network
> A separate line in the syllabus notes. Everything tested so far is about *types* and *format*; the allocation mechanism (router assigns a private address to each device on the LAN; ISP assigns the public address to the router) appears only inside router mark schemes, never as its own question.

> [!info] Security implications of public vs private, as an "explain" question
> The notes say "…and the implications for security". 9618 gets at this only through the routers bullet and the tick-table. An "explain why using private IP addresses within a LAN improves security" question sits directly on the syllabus wording.

---

## 2.1.15 Explain how a URL is used to locate a resource on the WWW, and the role of the DNS

> [!success] How a web browser uses a URL to access a web page
> Browser checks its cache; parses the URL into component parts; queries a DNS server for the IP address of the domain name; receives the matching IP; connects to the web server at that IP; requests the resource; renders and displays the result; stores the IP in cache. `9618_w25_qp_11_sc_7.c`

> [!warning] Describe how a URL is converted into its matching IP address (DNS resolution in detail)
> URL parsed to obtain the domain name; sent to the nearest DNS server; DNS holds a list of domain names and matching IP addresses; name resolver searches its database; if not found the request is forwarded to a **higher-level DNS**; the original DNS caches the returned address; error message if never found. 9618's single question credits the outline but not the hierarchy. `9608_s19_qp_11_sc_1.b`

> [!warning] Domain name vs IP address ("are they the same thing?")
> IP address is the physical address of the server; the domain name is a memorable form, linked to an IP address by DNS; the domain name is stable while the IP may be dynamic. `9608_s21_qp_13_sc_6.b`

> [!warning] Meaning of the parts of a URL
> Protocol (`http`), domain name (`cie.org.uk`), file/resource (`computerscience.html`). **Never tested in 9618**, despite the bullet literally being about how a URL locates a resource. `9608_w15_qp_13_sc_3.b.i`

> [!warning] Special characters in a URL (`%20`, `?`)
> `%20` encodes a space (32 denary) because spaces are not allowed; `?` separates the URL from its parameters. `9608_w15_qp_13_sc_3.b.ii`

> [!warning] Ordering the steps of a URL→DNS→web server sequence
> Sequencing/letter-matching format. `9608_w18_qp_13_sc_4.a`

> [!warning] Accessing a web page without using DNS
> Type the IP address instead of the URL. `9608_w18_qp_11_sc_2.a`

> [!info] This bullet has exactly one 9618 question (w25) — and it is the newest paper in the Legend
> Everything else here is 9608 or inference. Cambridge examined the whole bullet in one 4-marker in w25; the component parts (URL structure, DNS hierarchy and caching, what happens when the domain is not found) are still unexamined in 9618 and are the obvious follow-ups.

> [!info] Why DNS caching exists
> Credited as a mark point in `w25_qp_11_sc_7.c` ("checks its cache", "stored in the browser cache for future use") but never explained. "Explain why the browser and the DNS server cache IP addresses" (speed, reduced DNS traffic) is a clean 2-marker.

> [!abstract] What a URL is, and its three parts
> A **unique identifier for a web page** — the website address — deliberately text-based so it is easy to remember. Split into **protocol** (communication method for transferring data between client and server, e.g. `https`) · **domain name** (the name of the server where the resource is located) · **web page / file name** (the location of the file on that server). Matches the 9608-only question above and is still untested in 9618.

> [!abstract] The DNS hierarchy — root, TLD, authoritative
> Both series stop at "forwarded to a higher-level DNS". SME names the chain: the browser's request may reach a **root server**, which points to the correct **Top-Level Domain (TLD) server** (`.com`, `.org`), which points to the **authoritative DNS server** for that domain, which returns the correct IP address. The three server types appear in **no mark scheme in either series** — useful for understanding, but a 9618 answer only needs "passed to a higher-level DNS".

> [!abstract] DNS propagation
> When a domain is registered, or its server's IP address changes, the DNS must be updated — this spread of the update across the internet is called **DNS propagation** and takes time. Explains *why* caching has a cost as well as a benefit, and is named nowhere in the syllabus or the mark schemes.

> [!abstract] DNS as "the internet's phone book"
> Without DNS you would have to remember the IP address of every site. The analogy is not a mark point, but it is the one-line justification for the credited "a domain name is a memorable form of an IP address".
