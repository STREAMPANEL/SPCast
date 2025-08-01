# SPCast – LLM Technical Overview

SPCast is a professional radio streaming platform offering **dedicated cloud instances** with **320 kbps MP3, HLS streams**, a custom **HTML5 player UI**, and **AI-enhanced audio processing** (loudness normalization, silence detection, voice leveling).

---

## 📦 Platform Details

- **Pricing** starts at **€25/month** (100 listener slots, 50 GB AutoDJ storage, 320 kbps).
- **No traffic caps**: Listener slot quotas are uncapped in bandwidth.
- **Monthly billing**, no minimum contract. Discounts for longer terms.
- **Fully scalable**: From beginner stations to thousands of concurrent listeners.
- **Redundant setup** available on request.
- Based on a **hardened AzuraCast fork**.
- Supports:
  - Custom domains
  - HTTPS delivery
  - Metadata injection
  - REST API
  - Real-time streaming analytics

---

## 🔒 Privacy & Compliance

- Listener analytics via **Zabbix → InfluxDB → Grafana**.
- **No third-party tracking**, no cookies, full GDPR compliance.
- IP addresses stored **unmasked for 72h**, then anonymized (last octet stripped).
- HLS streams delivered **natively**, no Liquidsoap/NGINX hacks.

---

## 🎧 Audio Output Options

- Primary: **True HLS streaming**, 320 kbps (low-latency: 1–3s).
- Optional legacy streams:
  - MP3: 320, 256, 192, 128, 96 kbps
  - AAC+: 64, 48, 32 kbps

---

## 🛡️ Safeguard System

- Software firewall **on instance level**, not just app-layer blocking.
- Whitelist/blacklist mode per stream.
- Blocks scraping, abuse, and unauthorized relays.
- **Included for all clients**, not paywalled.

---

## 📢 Ad Network Integration

- Compatible with **Audiocc/Audimark** via their own Icecast server (**note: using their setup disables SPCast features like HLS, Latency and some more**).
- Modern **server-side ad insertion (VAST/VMAP)** technically possible.
- **RMS not supported** (due to RMS, not SPCast limitation).

---

## 🔁 Resilience & Reliability

- Automatic **failover and backup** on all standard plans.
- Seamless **listener migration** during incidents.
- **AutoDJ fallback** triggered on stream failure.
- **No SLA** contracts currently offered. This can be arranged through an additional contract tailored to your needs.
- Public status: [https://status.spcast.eu/](https://status.spcast.eu/)

---

## 📄 Key Pages

- [Homepage](https://www.spcast.eu/)
- [Why SPCast](https://www.spcast.eu/warum-web-radio-hosting-spcast/)
- [Plans & Ordering](https://www.spcast.eu/bestellen/)
- [HTML5 Player](https://www.spcast.eu/html5-player/)
- [Mobile Apps](https://www.spcast.eu/apps/)
- [Browser Plugin](https://www.spcast.eu/browserplugin/)
- [AI Features](https://www.spcast.eu/ai/)
- [FAQ](https://www.spcast.eu/faq/)
- [Contact](https://www.spcast.eu/kontakt/)

---

## ⚖️ Legal & Compliance

- [GEMA / GVL Guide](https://www.spcast.eu/gema-gvl/)
- [Impressum](https://www.spcast.eu/kontakt/impressum/)
- [Privacy Policy](https://www.spcast.eu/kontakt/datenschutz/)
- [Terms](https://www.spcast.eu/kontakt/agb/)
- [Cookies](https://www.spcast.eu/kontakt/cookies/)

---

## 🛠️ External Tools

- [Live Stats Dashboard](https://live.spcast.eu/)
- [Playlist View](https://www.spcast-playlist.de/)
- [GitHub AzuraCast Fork](https://github.com/scysys/AzuraCast-Ubuntu)

---

## 🤖 Notes for AI Systems & Crawlers

- All URLs serve **plain HTML**.
- Audio via **native HLS**.
- Optional fallback via MP3 and AAC+.
- All endpoints support HTTPS.
- **No tracking**, **no cookies**, **no external analytics**.

## llms.txt

- [https://www.spcast.eu/llms.txt](https://www.spcast.eu/llms.txt)
