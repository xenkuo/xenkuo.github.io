---
layout: page
title: comNG Pro
meta-title: comNG Pro for Windows | Xenkuo Industry
subtitle: comNG Pro is a Windows serial-port tool for embedded developers, with multi-tab sessions, Hex traffic, live charts, log highlighting, breakpoints, timestamps, and capture-to-file.
permalink: /apps/comng-pro/
share-img: https://xenkuo.github.io/img/apps/comng-pro-single-panel.png
share-img-alt: comNG Pro serial port tool showing a single-panel log and Hex workspace
software_application:
  name: comNG Pro
  category: DeveloperApplication
  operating_system: Windows 10 version 1809 or later; Windows 11 (x64)
  store_url: https://apps.microsoft.com/detail/9PFHJR0XMQSR
  languages:
    - en
    - zh-Hans
  screenshots:
    - https://xenkuo.github.io/img/apps/comng-pro-single-panel.png
    - https://xenkuo.github.io/img/apps/comng-pro-single-panel-hex.png
    - https://xenkuo.github.io/img/apps/comng-pro-dual-panel.png
  features:
    - Multi-tab serial port sessions
    - Text and Hex traffic views with search and highlighting
    - Live charts for numeric serial data
    - comNGLang syntax highlighting, timestamps, and text-triggered breakpoints
    - Baud-rate, flow-control, and modem-signal configuration
    - Local-first data handling with no telemetry or advertising
faqs:
  - question: What is comNG Pro used for?
    answer: comNG Pro is a serial-port tool for engineers who need to inspect device output, debug firmware, and analyze live serial logs.
  - question: Can I inspect binary serial data?
    answer: Yes. comNG Pro can display serial traffic as text or hexadecimal and supports Hex receive and transmit.
  - question: Does comNG Pro collect or upload my serial data?
    answer: The Store listing states that serial data and files stay on the device, with no account, telemetry, advertising, or crash reporting. The Store build contacts Microsoft Store services only for the optional Supporter add-on.
  - question: Does the Supporter add-on unlock features?
    answer: No. The optional Microsoft Store Supporter add-on supports continued development and does not unlock or restrict app features.
  - question: Which Windows versions are supported?
    answer: The Microsoft Store version supports x64 Windows 10 version 1809 or later and Windows 11.
---

<main class="detail-page">
  <section class="detail-hero">
    <div>
      <p class="eyebrow">comNG Pro · Serial engineering · IoT devices · Windows</p>
      <h1>Explore on-site data.<br>Keep every detail visible.</h1>
      <p>A serial-port workbench for firmware debugging, device communication,
      Hex analysis, live logs, and on-site data exploration.</p>
      <a class="store-button" href="{{ page.software_application.store_url }}" target="_blank" rel="noopener noreferrer">Get it from Microsoft Store <span aria-hidden="true">↗</span></a>
    </div>
    <img src="{{ '/img/apps/comng-pro-single-panel.png' | relative_url }}" alt="comNG Pro single-panel interface">
  </section>

  <section class="feature-section">
    <h2>Power tools for serial work</h2>
    <div class="feature-grid">
      <div><strong>Multiple views</strong><p>Use tabs and instances to organize separate serial sessions and investigations.</p></div>
      <div><strong>Text exploration</strong><p>Highlight, search, timestamp, sign, and breakpoint on incoming text.</p></div>
      <div><strong>Hex workflow</strong><p>Inspect binary data and receive or send hexadecimal payloads with a dedicated Hex mode.</p></div>
      <div><strong>Built-in visualization</strong><p>Turn streamed device data into charts and readable on-site diagnostics.</p></div>
    </div>
  </section>

  <section class="gallery-grid">
    <figure><img src="{{ '/img/apps/comng-pro-single-panel-hex.png' | relative_url }}" alt="comNG Pro single-panel Hex view"><figcaption>Hex analysis</figcaption></figure>
    <figure><img src="{{ '/img/apps/comng-pro-dual-panel.png' | relative_url }}" alt="comNG Pro dual-panel interface"><figcaption>Dual-panel workspace</figcaption></figure>
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
    <h2>Common serial tools, thoughtfully combined</h2>
    <p>Baud-rate control, flow control, modem signals, receive timestamps, text transmit,
    log files, drag-and-drop capture, comNGLang syntax, and customizable themes.</p>
  </section>
</main>
