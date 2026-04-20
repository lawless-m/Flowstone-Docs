# Rake

A [[rust]] [[cli-tools]] for raking over your own infrastructure: ingests nmap XML, normalises it into a stable inventory, and produces an HTML report flagging end-of-life software, insecure protocols, and changes between scans.

**Repo:** `/nonreplicated/Git/Rake`

Built for a ~250-host estate where regular nmap scans produce a pile of fingerprints that are laborious to read by hand. Rake stores everything with full history in [[cozordb]] (Cozo on [[redb]]), uses zone-based identity to keep DHCP churn out of the diff, and applies rule-based analyses driven by YAML config: EOL via endoflife.date, insecure-protocol signatures, role inference, snowflake detection, and scan-to-scan diffs. No exploits, no active probing beyond nmap — read-only inventory and reporting, single binary, one-shot invocation.
