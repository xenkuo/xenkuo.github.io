---
layout: page
title: MQTTi
meta-title: MQTTi for Windows | Xenkuo Industry
subtitle: MQTTi is a Windows MQTT 3.1.1/5.0 client for IoT developers with multi-broker sessions, TLS, searchable timeline, split view, and JSON, HEX, Base64, or CBOR payloads.
permalink: /apps/mqtti/
share-img: https://xenkuo.github.io/img/apps/dark-session.png
share-img-alt: MQTTi Windows MQTT client with a searchable message timeline
software_application:
  name: MQTTi
  category: DeveloperApplication
  operating_system: Windows 10 version 1809 or later; Windows 11 (x64)
  store_url: https://apps.microsoft.com/detail/9MW8721JW63G
  languages:
    - en
    - zh-Hans
  screenshots:
    - https://xenkuo.github.io/img/apps/dark-session.png
    - https://xenkuo.github.io/img/apps/dark-connections.png
    - https://xenkuo.github.io/img/apps/connection-editor.png
  features:
    - MQTT 3.1.1 and MQTT 5.0 over TCP or TLS
    - Multiple simultaneous broker sessions with side-by-side split view
    - Searchable and editable message timeline with copy and export
    - JSON, HEX, plain text, Base64, and CBOR payloads
    - QoS 0, 1, and 2, retained messages, and publish favorites
    - Local settings and DPAPI-encrypted saved passwords
faqs:
  - question: Which MQTT versions and transports does MQTTi support?
    answer: MQTTi supports MQTT 3.1.1 and MQTT 5.0 over TCP or TLS, with QoS 0, 1, and 2.
  - question: Which payload formats can I publish and inspect?
    answer: MQTTi supports JSON, HEX, plain text, Base64, and CBOR payloads.
  - question: Can I work with multiple brokers at once?
    answer: Yes. MQTTi keeps independent sessions for multiple broker connections and can show two sessions side by side.
  - question: Does MQTTi upload usage data?
    answer: No. MQTTi has no telemetry or analytics and does not upload usage data. Broker connections are initiated by the user; connection profiles and settings are stored locally.
  - question: Is MQTTi free to download?
    answer: Yes. MQTTi is free to download, with an optional Microsoft Store Supporter add-on.
  - question: Which Windows versions are supported?
    answer: The Microsoft Store listing supports x64 devices running Windows 10 version 1809 or later, and Windows 11.
---

<main class="detail-page">
  <section class="detail-hero">
    <div>
      <p class="eyebrow">MQTTi · MQTT 3.1.1 &amp; 5.0 · IoT development · Windows</p>
      <h1>Every MQTT session,<br>one clear timeline.</h1>
      <p>Debug device messages, MQTT integrations, and IoT telemetry with a
      purpose-built code-editor timeline.</p>
      <a class="store-button" href="{{ page.software_application.store_url }}" target="_blank" rel="noopener noreferrer">Get it from Microsoft Store <span aria-hidden="true">↗</span></a>
    </div>
    <img src="{{ '/img/apps/dark-session.png' | relative_url }}" alt="MQTTi session timeline">
  </section>

  <section class="feature-section">
    <h2>Built for active MQTT work</h2>
    <div class="feature-grid">
      <div><strong>Multi-session</strong><p>Keep several broker connections visible and switch between live sessions.</p></div>
      <div><strong>Readable timeline</strong><p>Searchable, selectable, editable traffic with JSON highlighting and copy/export.</p></div>
      <div><strong>Flexible payloads</strong><p>JSON, plain text, HEX, Base64, and CBOR sending and receiving.</p></div>
      <div><strong>Secure by design</strong><p>MQTT 5 properties, TLS, QoS, retained messages, and DPAPI-protected credentials.</p></div>
    </div>
  </section>

  <section class="gallery-grid">
    <figure><img src="{{ '/img/apps/dark-connections.png' | relative_url }}" alt="MQTTi connection manager"><figcaption>Connections</figcaption></figure>
    <figure><img src="{{ '/img/apps/light-session.png' | relative_url }}" alt="MQTTi in light mode"><figcaption>Light interface</figcaption></figure>
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
    <h2>From connection to payload</h2>
    <p>Manage subscriptions, save publish favorites, split two sessions side by side,
    and move between English and Simplified Chinese interfaces.</p>
  </section>
</main>
