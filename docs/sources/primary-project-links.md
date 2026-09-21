# Primary Project Link Verification

This record resolves source-listed projects that initially lacked an explicit primary link in the publicly visible Zhihu article. Links were checked on 2026-09-21 by reading the named project's repository or maintained project page.

| Source-listed name | Verified primary link | Evidence read | Catalog decision |
| --- | --- | --- | --- |
| SNS3 | <https://github.com/sns3/sns3-satellite> | The repository README identifies **Satellite Network Simulator 3 (SNS-3)** as a satellite-network extension to ns-3 and documents its companion modules. Reviewed at commit `b80ce75fdbb5bd250e04c53b73c3d9cabac3cd50` on branch `master`. | Retained as `SNS-3 (SNS3)` and classified as an ns-3 satellite-network extension. |
| gr-opssat | <https://github.com/esa/gr-opssat> | The ESA repository README describes applications for receiving, demodulating, and decoding the UHF signal of the OPS-SAT mission. Reviewed at commit `8f2f0f5e3f15e575c054c3b9bc1f245e800f3c50` on branch `master`. | Retained as a communications support tool; corrected from simulator to receiver/demodulator/decoder. |
| OpenLTE | <https://sourceforge.net/projects/openlte/> | The project's source README points to the maintained OpenLTE SourceForge project and describes LTE FDD SDR applications and test code. The accessible source mirror is <https://github.com/osh/openlte>, reviewed at commit `01251fb2ae1ae18c6cced21e0eee9d7c5e2205bf` on branch `master`. | Retained as general 3GPP LTE/SDR support tooling; corrected from satellite simulation. |
| FLoRaSat | <https://github.com/viveris/FLoRaSat> | The repository README defines FLoRaSat as an OMNeT++ discrete-event simulator for end-to-end satellite IoT simulations based on LoRa and LoRaWAN adaptations. Reviewed at commit `e3c073ec5b0ec897950b2ff5dea765cc4e638d6d` on branch `FLoRaSat_v4_ult`. | Retained as a satellite-IoT simulator. |

## Maintenance Rule

Use the project-maintained link above as the default entry point. Before replacing any link, verify that the destination is authoritative and update this record with the retrieval date, evidence, and reason for the change. Do not use a search-result URL or an unverified fork as a primary project link.
