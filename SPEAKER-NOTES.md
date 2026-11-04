# Speaker notes: Flatcar Container Linux, Growing the Cloud Native OS Ecosystem

Lightning talk, 5 minutes, no Q&A. Target about 4:30. Times are cumulative.

## Slide 1: Cover (0:00 - 0:20)

"Hi everyone, I'm Jan, a Flatcar maintainer and software engineer at Microsoft. In five minutes: where the project stands in the CNCF, how we secure what we ship, and where you can jump in."

## Slide 2: Growing in the CNCF (0:20 - 1:20)

"Flatcar is a CNCF incubating project, and graduation is on our public roadmap. It is a minimal, immutable OS built for containers, and it runs Kubernetes nodes on the major clouds and on bare metal.

We ship through four channels: Alpha, Beta, Stable and LTS. Before each release the full test suite runs across the supported clouds, on both amd64 and arm64.

And the OS keeps getting more modular. Docker and containerd already ship as systemd-sysexts, and Podman and the NVIDIA drivers are official opt-in ones. The core stays small, the ecosystem grows around it."

## Slide 3: Supply chain integrity (1:20 - 2:50)

Walk the pipeline left to right.

"Here is how an update gets to your node. Every change is reviewed by a maintainer before it merges. Everything is built from source in an ephemeral environment, never from pre-built binaries. The build produces an SPDX SBOM, generated with syft and published signed next to every image, as `flatcar_production_image_sbom.json`, and it produces SLSA provenance, with per-package provenance shipped inside the image under `/usr/share/SLSA`. The update image is signed with a key that lives in an HSM, in an air-gapped environment. And on your node, dm-verity checks the read-only `/usr` partition at every boot.

Our own assessment is SLSA Level 3, and we track the remaining Level 4 items in the open.

Coming soon: we will publish VEX files with every release, so besides the SBOM you get a machine-readable statement of which known CVEs actually affect that release. What is next after that: a TPM-based chain of trust for the build infrastructure, and a more scalable release signing process."

## Slide 4: Roadmap, and where you can help (2:50 - 4:00)

"The roadmap is public in the Flatcar repo. Right now: CNCF graduation, systemd-sysext and confext, and the TPM and Secure Boot work. Next: full-disk encryption and a more automated release pipeline.

Where do you come in? There are labelled good first issues and help-wanted items, docs that need love, new platforms and releases that need testing, and sysext images that need maintainers.

Come find us this week at the Project Pavilion, kiosk P-8A in Hall 5, Cosmic Canyon Zone. The Flatcar shifts are Tuesday 3 to 7 p.m., Wednesday 1:55 to 5, and Thursday 12:25 to 2."

## Slide 5: Takeaways (4:00 - 4:30)

"Secure by design, open by default, and come build it with us. We have office hours every second Thursday and a dev sync every fourth. Everything is at flatcar.org and github.com/flatcar, and we are on Discord. Thank you!"

## Reminders

- Kiosk shifts: Tue 3:00-7:00 PM, Wed 1:55-5:00 PM, Thu 12:25-2:00 PM MST. Early setup: Mon 8:00-17:30, or 9:00-10:00 on the day.
- Arrive 15 min early, check in at the back, sit stage right in the reserved seats.
- Own laptop and HDMI adapter. No clicker. Stay near the podium (recorded).
- No Q&A, no swag or promo.
- If running long, cut the "on both amd64 and arm64" clause on slide 2 and the sysext paragraph.
- Facts to re-check before the day: still "incubating" (graduation may have moved), SLSA level wording. SBOM was verified on the release server (signed `flatcar_production_image_sbom.json`).
