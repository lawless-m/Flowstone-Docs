# Snazzy

A "QNAP custom Linux" project — documenting the process of replacing QNAP stock firmware with [[Debian]] on a TS-412, while keeping the production TS-431X on the official QTS for 10GbE networking.

**Repo:** `~/Git/Snazzy`
**Themes:** [[Debian]], (NAS firmware)

Target hardware is a QNAP TS-412, an ARM Kirkwood NAS; Debian 10 (buster) is the last version supporting that architecture, and it's end-of-life, but the goal is full control rather than long-term maintenance. Ships a hardware spec doc, a TS-412 original-firmware backup procedure, a TS-412 Debian installation guide, and a services-planning doc. Project status checkboxes at last touch are all unticked — backup, install, configure, document — so this is planning-and-documentation stage. References Martin Michlmayr's Kirkwood/QNAP guide as the canonical upstream. Sibling to [[NASty]], which is a more generic embedded-flash / PXE-boot NAS hack, and to [[tplinkac750]] if it turns out to be router-firmware work.

## Related

- [[NASty]] — sibling embedded-Linux / NAS firmware hack
- [[tplinkac750]] — likely sibling hardware project (TP-Link AC750 router)
- [[Debian]]
