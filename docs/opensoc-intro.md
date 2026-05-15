# OpenSOC Intro

Source post: https://iamb4uc.xyz/post/opensoc-intro/

OpenSOC is a SOC lab series focused on building a security operations environment with a clear paper trail. The goal is to document how the lab is built and why decisions were made, instead of letting alerts, screenshots, notes, dashboards, and investigation context disappear across random places.

## Project Idea

The lab should stay small enough to understand. It should be modular so it can grow without rebuilding everything from scratch.

The working loop is:

1. Collect telemetry.
2. Detect suspicious activity.
3. Alert with context.
4. Preserve evidence.
5. Review what happened.
6. Improve the lab and detections.

## Current Direction

The first lab direction starts with:

- Wazuh as the SIEM.
- Linux endpoint monitoring with the Wazuh agent.
- `auditd`.
- `osquery`.
- FleetDM OSS.
- Basic detections.
- Alerting.
- Evidence collection.

These items are part of the project direction from the intro post. Only the Wazuh server setup has a dedicated setup doc right now.

## Future Direction

The intro post mentions that the lab may later grow into:

- Suricata.
- Zeek.
- SOAR.
- Windows agents.
- macOS agents.
- Splunk.

These are intentionally not documented as setup steps yet.
