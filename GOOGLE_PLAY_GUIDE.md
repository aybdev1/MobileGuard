# MobileGuard — Google Play Deployment Guide

---

## App Positioning vs Competitors

| Feature | MobileGuard | NetGuard | AdGuard | Blokada | RethinkDNS |
|---|---|---|---|---|---|
| DNS-only VPN | ✓ | ✓ | ✓ | ✓ | ✓ |
| On-device AI anomaly detection | ✓ | ✗ | ✗ | ✗ | ✗ |
| 4 ML models (DCL/CLG/TRF/AE) | ✓ | ✗ | ✗ | ✗ | ✗ |
| Spyware scanner | ✓ | ✗ | ✗ | ✗ | ✗ |
| Real-time connection monitor | ✓ | partial | ✗ | ✗ | partial |
| Network device scanner (IoT) | ✓ | ✗ | ✗ | ✗ | ✗ |
| Forensic encrypted log | ✓ | ✗ | ✗ | ✗ | ✗ |
| Live attack map | ✓ | ✗ | ✗ | ✗ | ✗ |
| Customizable Quick Access | ✓ | ✗ | ✗ | ✗ | ✗ |
| AI auto-block with confidence | ✓ | ✗ | ✗ | ✗ | ✗ |
| DNS entropy / DGA detection | ✓ | ✗ | ✗ | ✗ | ✗ |
| No root required | ✓ | ✓ | ✓ | ✓ | ✓ |
| Free base tier | ✓ | ✓ | freemium | ✓ | ✓ |

**Unique value:** MobileGuard is the only consumer Android app combining DNS-level ad/tracker blocking with on-device machine learning anomaly detection, spyware scanning, and IoT network intelligence — all without root access.

---

## Google Play Store Listing

### App Name
**MobileGuard — AI DNS Firewall**

### Short Description (80 chars)
```
AI-powered DNS firewall: block ads, trackers, spyware & detect threats.
```

### Full Description (4000 chars max)
```
🔒 MOBILEGUARD — AI-POWERED DNS FIREWALL & THREAT DETECTOR

MobileGuard is a professional-grade mobile security application combining DNS-level network 
protection with on-device artificial intelligence to detect and block threats, ads, trackers, 
and malicious domains — all without requiring root access.

─── WHAT MAKES IT DIFFERENT ───────────────────────────────────────────
Unlike basic ad blockers, MobileGuard includes a full anomaly detection engine running 
4 machine learning models directly on your device. No data ever leaves your phone for analysis.

─── CORE PROTECTION ────────────────────────────────────────────────────
✅ DNS Firewall — blocks ads, trackers, and malware at the DNS level
✅ 150,000+ domains blocked from premium blocklists
✅ Google Ads, YouTube pre-roll ads, DoubleClick, teads, Criteo blocked
✅ Survives Doze mode — WakeLock + WifiLock keeps protection active
✅ Block-on-boot support — protection restarts automatically

─── AI THREAT DETECTION ────────────────────────────────────────────────
🤖 4 detection models you can choose from:
  • DCL (Anomaly Engine) — general-purpose DNS anomaly detection
  • CLG (Graph Neural Network) — detects coordinated C2 infrastructure
  • TRF (Mini Transformer) — catches slow APT-style hidden threats
  • AE (Adaptive Autoencoder) — learns YOUR traffic patterns personally

Adjustable confidence threshold (10–99%). Auto-block only at high confidence.
Trusted domains (Google, Apple, Microsoft, Amazon) are whitelisted to prevent false positives.

─── NETWORK INTELLIGENCE ───────────────────────────────────────────────
📡 IoT Device Scanner — discover all devices on your Wi-Fi network
📡 Connection Monitor — see every active TCP/UDP connection in real time
📡 Live Attack Map — visualize threats geographically
📡 Packet Inspector — deep DNS analysis with entropy and DGA detection
📡 DNS Leak Detector — verify your VPN isn't leaking to your ISP
📡 Port Scanner — audit open ports on your router and network

─── PRIVACY & SECURITY ─────────────────────────────────────────────────
🛡 Spyware Detector — scans for 14 known stalkerware apps and suspicious permissions
🛡 Forensic Log — AES-256 encrypted event log, stored locally only
🛡 No telemetry — zero analytics, no crash reporting, no cloud
🛡 All AI processing on-device — your DNS queries never leave your phone
🛡 Coalition Against Stalkerware compatible — detects covert surveillance tools

─── DASHBOARD & ANALYTICS ──────────────────────────────────────────────
📊 24-hour traffic charts (blocked vs allowed)
📊 Risk distribution donut, category breakdown, hourly heatmap
📊 Top blocked domains with proportion bars
📊 Per-app DNS query correlation and risk scoring
📊 Real-time threat counter and active alert system
📊 Customizable Quick Access — choose exactly which tools appear on your home screen

─── PERMISSIONS USED ───────────────────────────────────────────────────
• BIND_VPN_SERVICE — required to create the DNS tunnel
• FOREGROUND_SERVICE — keeps protection running
• WAKE_LOCK — prevents Doze from killing the tunnel
• INTERNET — loads blocklist updates
• POST_NOTIFICATIONS — security alerts (can be disabled)

No camera, microphone, location, or contact permissions used.

─── TECHNICAL DETAILS ──────────────────────────────────────────────────
• Min Android version: 8.0 (API 26)
• DNS-only VPN (port 53) — no traffic inspection, no TLS interception
• All filtering is local and on-device
• Custom blocklist URL support (hosts format, AdBlock Plus format)
```

### Category
**Tools** (primary) / **Security** (secondary tag)

### Content Rating
**Everyone** — no mature content

### Tags
`vpn, firewall, ad blocker, privacy, security, dns, tracker blocker, parental controls, network monitor, malware, spyware`

---

## Revenue Strategy

### Free Tier (default)
- Full DNS blocking
- 1 detection model (DCL)
- Basic analytics
- Network scanner
- In-app AdMob banners (320×50 in Quick Access area)
- Interstitials on: VPN start, every 4th navigation, every 10 threats

### Premium Tier — €2.99/month or €19.99/year (Google Play Billing)
- All 4 AI detection models
- Advanced Analytics (24h charts, risk heatmap, app insight)
- Forensic encrypted log
- Live Attack Map
- Spyware Detector
- Connection Monitor
- Custom blocklist URLs
- Remove all ads
- Priority blocklist updates

### Estimated Revenue (100K DAU)
- Free 80% → AdMob: ~$2-4 CPM, 3 impressions/day = ~$50-100/day
- Premium 5% (5,000 users × €2.99/month) = ~$14,950/month
- **Total realistic: $20-30K/month at 100K DAU**

---


## Privacy Policy Requirements (mandatory for VPN apps)


1. **No traffic inspection**: MobileGuard only intercepts DNS queries (domain names), never URL paths, payload content, or encrypted data.
2. **No data collection**: No DNS queries, no usage analytics, no personal data is transmitted to any server.
3. **Local-only processing**: All AI detection runs on-device. The forensic log is stored encrypted on-device only.
4. **VPN permission usage**: Solely used to create a local DNS filter tunnel, not for privacy circumvention.



