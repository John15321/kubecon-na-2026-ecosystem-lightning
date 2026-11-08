# Speaker notes: Flatcar Container Linux, Growing the Cloud Native OS Ecosystem

Lightning talk, 5 minutes, no Q&A. Target about 4:30. Times are cumulative.

## Slide 1: Cover (0:00 - 0:20)

"Hi everyone, I'm Jan, a Flatcar maintainer and software engineer at Microsoft. In five minutes: our mission, what we are doing now, and where you can jump in."

## Slide 2: Our mission (0:20 - 1:10)

"Flatcar's mission is simple: a boring, secure OS for running containers. Today we describe everything in our stack as code, except the operating system. That gap is the problem: general-purpose distros drift over time and need patching by hand. Our answer is Operating System as Code. We made the OS immutable: `/usr` is read-only and verified at every boot, and updates are atomic with automatic rollback. It is cloud agnostic: it runs Kubernetes nodes on every major cloud and on bare metal. It is fully free and open-source, and community-driven. And it is secure by default: minimal, signed, and tested before every release."

## Slide 3: Where we are today (1:10 - 2:10)

"Where are we today? In a good place. In 2024 Flatcar became the first operating system distribution the CNCF accepted, at incubating level, which in CNCF terms means stable and used successfully in production. It is trusted by companies like Adobe, Giant Swarm, Wipro and 1&1, and it runs on public clouds, bare metal and private clouds alike. It sits behind several managed Kubernetes services and works with Cluster API. It is stable and reliable: atomic updates with rollback, and every release tested. And the community is over 600 contributors and growing."

## Slide 4: What we are doing now, and what is next (2:10 - 4:00)

"Flatcar is a CNCF incubating project, and graduation is on our public roadmap. To fit the CNCF governance model, we are adding a Steering Committee and a Technical Committee, so decisions are shared and not tied to a few people. We are also redoing our maintainer roles and structure, because the number of maintainers and subprojects keeps growing. And we are aligning more closely with our upstream, Gentoo, by tracking its packages more tightly.

We did an overhaul of our infrastructure, and we are now expanding our tests and processes, and the list of platforms we support. Every release is tested across clouds before it ships. On security, we are publishing VEX files with our releases, so you know which known CVEs actually affect them, and we are making our security triage more automated, with the help of AI.

Next: a TPM-based chain of trust, scalable release signing, and a more automated release pipeline. The roadmap is public in the Flatcar repo. Where do you come in? Labelled good first issues and help-wanted items, docs that need love, new platforms and releases that need testing, and sysext images that need maintainers."

## Slide 5: Find us at the kiosk (4:00 - 4:30)

"Come find us this week at the Project Pavilion, kiosk P-8A, Hall 5, Cosmic Canyon Zone. The shifts are Tuesday 3 to 7 p.m., Wednesday 1:55 to 5, and Thursday 12:25 to 2. Scan the QR code to join our Discord, and we also have office hours every second Thursday and a dev sync every fourth. Everything is at flatcar.org and github.com/flatcar. Thank you!"

## Reminders

- Kiosk shifts: Tue 3:00-7:00 PM, Wed 1:55-5:00 PM, Thu 12:25-2:00 PM MST. Early setup: Mon 8:00-17:30, or 9:00-10:00 on the day.
- Arrive 15 min early, check in at the back, sit stage right in the reserved seats.
- Own laptop and HDMI adapter. No clicker. Stay near the podium (recorded).
- No Q&A, no swag or promo.
- If running long, cut the Gentoo sentence on slide 4.
- Facts to re-check before the day: slide 3 numbers (600+ contributors is from the Oct 2024 CNCF post), adopter names against ADOPTERS.md; AI triage and VEX wording matches what is actually shipping; still "incubating" (graduation may have moved).
