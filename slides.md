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

# Our mission: a boring, secure OS for containers

- **The problem:** everything in our stack is code except the OS
- **Our answer:** **Operating System as Code**
- **Immutable:** read-only `/usr`, verified at boot, atomic updates with rollback
- **Cloud agnostic:** runs Kubernetes nodes on every major cloud and bare metal
- **Fully open:** free and open-source, community-driven
- **Secure by default:** minimal, signed, tested before every release

---

# Where we are today

- First OS distribution accepted into the CNCF, at **incubating** level
- Trusted in production: **Adobe, Giant Swarm, Wipro, 1&1** and many more
- Used on public clouds, **bare metal** and private clouds alike
- Behind several **managed Kubernetes** services, with Cluster API support
- **Stable and reliable:** atomic updates with rollback, every release tested
- **600+ contributors** and a growing community

---

# What we are doing now, and what is next

- CNCF **incubating**, with graduation on the roadmap
- New **Steering and Technical committees**, reworked **maintainer roles**
- Closer alignment with our **Gentoo** upstream packages
- **Infrastructure overhaul** done, now expanding tests, processes and **platforms**
- Publishing **VEX files** and automating security triage with **AI**
- **Next:** TPM chain of trust, scalable release signing, a more automated release pipeline
- **You:** good first issues, docs, testing new platforms, sysext images

---

<!-- _class: closing -->
<!-- _paginate: false -->

<style scoped>section.closing { padding-bottom: 36px; } section.closing p.closing-meetings { margin-bottom: 12px; }</style>

# Find us at<br>Project Pavilion, kiosk P-8A

<p class="closing-qr-caption"><img src="assets/logos/external/discord-white.svg" alt=""> Join our Discord!</p>

<p class="closing-links">
  <a href="https://flatcar.org"><img src="assets/logos/flatcar-logotype/icon/white/flatcar-icon-white.svg" alt=""> flatcar.org</a>
  <a href="https://github.com/flatcar"><img src="assets/logos/external/github-white.png" alt=""> github.com/flatcar</a>
  <a href="https://chat.flatcar.org"><img src="assets/logos/external/discord-white.svg" alt=""> chat.flatcar.org</a>
</p>

<p class="closing-meetings">
  <span><strong>Office hours</strong> · every 2nd Thu, 16:30 CEST</span>
  <span><strong>Dev sync</strong> · every 4th Thu, 16:30 CEST</span>
</p>

<p class="closing-cta" style="font-size: 30px; line-height: 1.4; max-width: 1100px"><strong>Hall 5, Cosmic Canyon Zone</strong><br><strong>Shifts (MST):</strong> Tue 3-7 PM, Wed 1:55-5 PM, Thu 12:25-2 PM</p>
