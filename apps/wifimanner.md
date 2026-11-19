---
layout: page
title: Wi-Fi Manner
meta-title: Wi-Fi Manner for Windows | Xenkuo Industry
subtitle: Wi-Fi Manner is a Windows Wi-Fi analyzer for embedded engineers. Scan access points and inspect SSID, BSSID, channel, band, channel width, RSSI, and signal strength.
permalink: /apps/wifimanner/
share-img: https://xenkuo.github.io/img/apps/wifimanner-live-scan.png
share-img-alt: Wi-Fi Manner live Wi-Fi scan showing access points, channels, and signal strength
software_application:
  name: Wi-Fi Manner
  category: DeveloperApplication
  operating_system: Windows 10 version 1809 or later; Windows 11 (x64)
  store_url: https://apps.microsoft.com/detail/9NBT5F55QT68
  screenshots:
    - https://xenkuo.github.io/img/apps/wifimanner-live-scan.png
    - https://xenkuo.github.io/img/apps/wifimanner-airtime.png
    - https://xenkuo.github.io/img/apps/wifimanner-connection.png
  features:
    - Live Wi-Fi network scanning
    - Access point SSID, BSSID, channel, band, and channel-width details
    - RSSI and signal-strength indicators
    - Filters for 2.4 GHz, 5 GHz, and 6 GHz networks
faqs:
  - question: What information does the live scan show?
    answer: The live scan lists SSID, BSSID, channel, band, channel width, RSSI, and a signal-strength indicator for nearby access points.
  - question: Which Wi-Fi bands can I filter?
    answer: The live scan provides filters for 2.4 GHz, 5 GHz, and 6 GHz networks, as well as an all-bands view.
  - question: Can Wi-Fi scanning refresh automatically?
    answer: Yes. Wi-Fi Manner provides a Scan Now action and an Auto Refresh option.
  - question: Which Windows versions are supported?
    answer: The app targets x64 Windows 10 version 1809 or later and Windows 11.
---

<main class="detail-page">
  <section class="detail-hero wifi-detail">
    <div>
      <p class="eyebrow">Wi-Fi Manner · Wireless analysis · IoT engineering · Windows</p>
      <h1>See the connection.<br>Understand the traffic.</h1>
      <p>Inspect nearby access points in real time, compare their channels and
      signal levels, and validate wireless conditions for embedded devices.</p>
      <a class="store-button" href="{{ page.software_application.store_url }}" target="_blank" rel="noopener noreferrer">Get it from Microsoft Store <span aria-hidden="true">↗</span></a>
    </div>
    <img src="{{ '/img/apps/wifimanner-live-scan.png' | relative_url }}" alt="Wi-Fi Manner live Wi-Fi scan">
  </section>

  <section class="feature-section">
    <h2>Live wireless diagnostics</h2>
    <div class="feature-grid">
      <div><strong>Access point details</strong><p>Compare SSID, BSSID, channel, band, and channel width in one sortable view.</p></div>
      <div><strong>Signal visibility</strong><p>Review RSSI values and signal bars while scanning nearby networks.</p></div>
      <div><strong>Band filters</strong><p>Focus the live scan on 2.4 GHz, 5 GHz, or 6 GHz networks.</p></div>
      <div><strong>Refresh controls</strong><p>Run a scan on demand or enable automatic refresh while monitoring an environment.</p></div>
    </div>
  </section>

  <section class="gallery-grid wifi-gallery" aria-label="Wi-Fi Manner screenshots">
    <figure><img src="{{ '/img/apps/wifimanner-airtime.png' | relative_url }}" alt="Wi-Fi Manner airtime analysis"><figcaption>Capture airtime analysis</figcaption></figure>
    <figure><img src="{{ '/img/apps/wifimanner-connection.png' | relative_url }}" alt="Wi-Fi Manner connection analysis"><figcaption>Device connection analysis</figcaption></figure>
  </section>

  <section class="faq-section">
    <h2>Frequently asked questions</h2>
    <div class="faq-list">
      {% for item in page.faqs %}
      <details>
        <summary>{{ item.question | escape }}</summary>
        <p>{{ item.answer | escape }}</p>
      </details>
      {% endfor %}
    </div>
  </section>

  <section class="detail-footer">
    <h2>Built for practical radio diagnostics</h2>
    <p>Wi-Fi Manner surfaces Windows WLAN scan data in a clear, sortable view for
    embedded development, wireless troubleshooting, and field diagnostics.</p>
  </section>
</main>
