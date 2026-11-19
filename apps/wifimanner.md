---
layout: page
title: WiFi Manner
subtitle: Live and offline Wi-Fi analysis for Windows
css:
  - "/css/apps.css"
permalink: /apps/wifimanner/
---

<main class="detail-page">
  <section class="detail-hero wifi-detail">
    <div>
      <p class="eyebrow">Wi-Fi analysis · Windows</p>
      <h1>See the connection.<br>Understand the traffic.</h1>
      <p>Explore nearby networks in real time and analyze captured Wi-Fi activity,
      device lifecycles, and protocol timelines offline.</p>
      <a class="button-primary" href="https://github.com/xenkuo/wifimanner" target="_blank" rel="noopener">View source</a>
    </div>
    <div class="wifi-detail-mock">
      <div class="wifi-toolbar"><span class="wifi-dot"></span><strong>WiFi Manner</strong></div>
      <div class="wifi-detail-chart">
        <div class="timeline-y"><span>Beacon</span><span>Probe</span><span>Auth</span><span>EAPOL</span><span>TCP</span><span>DNS</span></div>
        <div class="timeline-x">
          <i class="line-a"></i><i class="line-b"></i><i class="line-c"></i><i class="line-d"></i><i class="line-e"></i>
        </div>
      </div>
    </div>
  </section>

  <section class="feature-section">
    <h2>Two views of the wireless layer</h2>
    <div class="feature-grid">
      <div><strong>Live scanning</strong><p>Inspect SSID, BSSID, channel, band, RSSI, and signal quality with sortable filters.</p></div>
      <div><strong>PCAPNG analysis</strong><p>Process capture files into device, access-point, session, and protocol views.</p></div>
      <div><strong>Connection lifecycle</strong><p>Follow probe, authentication, association, EAPOL handshake, and subsequent traffic.</p></div>
      <div><strong>Protocol timeline</strong><p>Trace packet activity across 802.11 and application protocol layers.</p></div>
    </div>
  </section>

  <section class="detail-footer">
    <h2>Built for practical radio diagnostics</h2>
    <p>WiFi Manner is designed around real capture data and Windows-native tools:
    live WLAN data through the system API and offline pcapng processing without
    a GPL runtime dependency.</p>
  </section>
</main>
