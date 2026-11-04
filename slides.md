---
marp: true
theme: flatcar
paginate: true
size: 16:9
title: "Flatcar Container Linux: Growing the Cloud Native OS Ecosystem"
author: Jan Bronicki
---

<!-- _class: cover -->
<!-- _paginate: false -->

# Flatcar Container Linux: Growing the Cloud Native OS Ecosystem

## Project Lightning Talk, KubeCon + CloudNativeCon North America 2026

<div style="display: flex; align-items: center; gap: 28px; margin: 28px 0 10px 0">
  <img src="assets/photo/individual_photos/jan-bronicki.jpeg" alt="Jan Bronicki" style="width: 150px; height: 150px; object-fit: cover; border-radius: 6px">
  <div style="font-size: 24px; line-height: 1.45">
    <strong style="font-size: 32px">Jan Bronicki</strong><br>
    Flatcar Maintainer, Software Engineer at Microsoft<br>
    <span style="display: inline-flex; align-items: center; gap: 8px; margin-right: 24px"><img src="assets/logos/external/github-white.png" alt="GitHub" style="height: 24px; width: 24px">@John15321</span>
    <span style="display: inline-flex; align-items: center; gap: 8px"><img src="assets/logos/external/linkedin-white.svg" alt="LinkedIn" style="height: 24px; width: 24px">jan-bronicki</span>
  </div>
</div>

---

# Growing in the CNCF

- CNCF **incubating** project, with graduation on the roadmap
- Runs Kubernetes nodes on the major clouds and bare metal
- Alpha, Beta, Stable and LTS channels, each release tested across clouds before it ships
- Extensible by design: Docker, containerd, Podman and GPU drivers ship as **sysexts**

---

# Supply chain integrity

<img style="width: 100%; margin-top: 0" src="assets/diagrams/supply-chain.svg" alt="Pipeline: reviewed source, ephemeral build, SLSA provenance, HSM-signed update, dm-verity checked at boot">

- Signed **SPDX SBOM** published with every image
- Assessed at **SLSA Level 3**, per-package provenance in `/usr/share/SLSA/`
- Coming: **VEX files** with every release, so you know which CVEs matter
- Next: TPM chain of trust, scalable release signing

---

# Roadmap, and where you can help

- **Now:** CNCF graduation, systemd-sysext and confext, TPM and Secure Boot
- **Next:** full-disk encryption, a more automated release pipeline
- **You:** good first issues, docs, testing new platforms, sysext images
- Find us: **Project Pavilion, kiosk P-8A**, Hall 5, Cosmic Canyon Zone

---

<!-- _class: closing -->
<!-- _paginate: false -->

# Secure by design.<br>Open by default.<br>Come build it with us.

<p class="closing-qr-caption"><img src="assets/logos/external/discord-white.svg" alt=""> Join our Discord!</p>

<p class="closing-links">
  <a href="https://flatcar.org"><img src="assets/logos/flatcar-logotype/icon/white/flatcar-icon-white.svg" alt=""> flatcar.org</a>
  <a href="https://github.com/flatcar"><img src="assets/logos/external/github-white.png" alt=""> github.com/flatcar</a>
  <a href="https://discord.gg/PMYjFUsJyq"><img src="assets/logos/external/discord-white.svg" alt=""> discord.gg/PMYjFUsJyq</a>
</p>

<p class="closing-meetings">
  <span><strong>Office hours</strong> · every 2nd Thu, 16:30 CEST</span>
  <span><strong>Dev sync</strong> · every 4th Thu, 16:30 CEST</span>
</p>
