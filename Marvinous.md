# Marvinous

A [[Rust]] server monitoring tool with the personality of Marvin the Paranoid Android — collects hardware metrics via IPMI, SMART, and nvidia-smi, then writes hourly reports through [[Ollama]].

**Repo:** `~/Git/Marvinous`
**URL:** `https://dw.ramsden-international.com/marvinous/`

Reads 80+ IPMI BMC sensors, SMART drive health, GPU stats, and system logs, then sends the lot to Qwen for sardonic analysis with severity ratings (OK/WATCH/CONCERN/CRITICAL). Web dashboard on port 9090 with colour-coded reports and manual collection triggers. Daily summaries consolidate and archive hourly reports. Runs as systemd timers. Deployed on [[Dw.ramsden-International.com]].
